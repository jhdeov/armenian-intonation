I generally followed the strategy in the [Interlingual-MFA](https://github.com/jhdeov/interlingual-MFA) repo.

* I didn’t use any beams, but just speaker adaptation. 
*	The original dictionary was turned to lowercase
*	I ran the Armenian data against english_mfa, spanish_mfa, french_mfa, and german_mfa. These models were trained over 1000s of hours of data.
*	I kept a copy of the phone_mapping that I used. For non-English, I suspect that there are probably more accurate possible mappings. For example, Armenian /ʁ, ɾ, r/ are all mapped to French /ʁ/. You can see French’s phones and other languages’ phones here [Fr](https://mfa-models.readthedocs.io/en/latest/dictionary/French/French%20MFA%20dictionary%20v2_0_0a.html#french-mfa-dictionary-v2-0-0a), [Gr](https://mfa-models.readthedocs.io/en/latest/dictionary/German/German%20MFA%20dictionary%20v2_0_0a.html#german-mfa-dictionary-v2-0-0a), [Sp](https://mfa-models.readthedocs.io/en/latest/dictionary/Spanish/Spanish%20MFA%20dictionary%20v2_0_0a.html#spanish-mfa-dictionary-v2-0-0a), [En](https://mfa-models.readthedocs.io/en/latest/dictionary/English/English%20MFA%20dictionary%20v2_0_0a.html#english-mfa-dictionary-v2-0-0a).
*	I also ran an Armenian-based aligner [Hy](https://github.com/jhdeov/armenianMFA/) just for fun, no beam changes
*	Below are the snippets that I used. 

# Code

1) convert dictionary
> python convertPronDict.py /word-pronunciations-EA.tsv  /phoneMappingFr.txt /Users/Hovsep/Desktop/pronDictIntermediate.txt

2) validate dictionary
> mfa validate /EA /pronDictIntermediate.txt french_mfa --ignore_acoustics

3) align
> mfa align /EA  /pronDictIntermediate.txt  french_mfa /EA_Fr --clean --overwrite --Speaker_characters=4

4) convert alignments
> python convertAlignments.py wordTranscriptions.pkl  /EA_Fr

# TODOs
* It would be nice to play with inter-annotator agreement via these aligners
* Perhaps the non-English models can be improved by one of you refining the phone-mapping files, by using knowledge of European phonetics wrt to English/Armenian
* The pauses may be [problematic](https://montreal-forced-aligner.readthedocs.io/en/latest/user_guide/corpus_creation/training_dictionary.html#silence-probability-and-correction-factors).

