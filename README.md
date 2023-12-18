# Speech corpus of Armenian question-answer dialogues

This is a corpus of elicited controlled speech. The stimuli was a sequence of dialogues with intermittent fillers. This repository is for only the stimuli. The stimuli was designed to elicit intonation patterns for questions and answers in two Armenian dialects: Western Armenian (WA) and Eastern Armenian (EA). The recordings can be used for topics like intonation prosody, forced alignment, or ASR (Automatic Speech Recognition). 


The dataset is is open-access at 8,852 dialogues, consisting of 23,711 utterances (individual sound files), for a total of 2.7GB and 8.5hrs.  Each utterance has a sound file, a Praat TextGrid (with full linguistic annotation), and text file that has orthographic forms for easier ASR uses. Pronunciation dictionaries are provided for ASR or forced alignment purposes as well. We genereted a forced alignment for these recordings using a cross-language alignment thanks to [Interlingual-MFA](https://github.com/jhdeov/interlingual-MFA). See the [Alignments folder](alignments).


If you use the data in any way, please cite us as:

> Chakmakjian, Samuel and Hossep Dolatian. 2022. *Speech corpus of Armenian question-answer dialogues*. [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7088365.svg)](https://doi.org/10.5281/zenodo.7088365)  


# Stimuli design
## Overview
A dialogue is made up of at least a question (Q) and an answer (A). Some dialogues include an interjection (I) and a negated verb (N). We call all these elements (Q, A, I, N) utterances. 


The question and answer were SOV sentences. The dialogues were of three types, each with a different position of focus. Focus was either on the subject, object, or verb. Dialogues also varied in the choice of the object word. The object word could have either final stress, penultimate stress, or initial stress. 

File utterance-metadata (in [Excel](utterance-metadata.xlsx) and [TSV](utterance-metadata.tsv) versions) has metadata on the conditions for each recorded utterance.

## Dialogue types and focus type
The following is the template for the dialogues. The actual recordings vary in the TARGET word for the object. Note that for Western Armenian, our speakers were from Syria. They usually didn’t aspirate. 



<table class="tg">
<thead>
  <tr>
    <th class="tg-0lax">Type</th>
    <th class="tg-0lax"></th>
    <th class="tg-0lax" colspan="3">&nbsp;&nbsp;&nbsp;<br>&nbsp;&nbsp;&nbsp;Subject focus dialogue</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0lax">Question</td>
    <td class="tg-0lax">IPA (WA)</td>
    <td class="tg-0lax">*ov*   </td>
    <td class="tg-0lax">TARGET   </td>
    <td class="tg-0lax">əsɑv   </td>
  </tr>
  <tr>
    <td class="tg-0lax"></td>
    <td class="tg-0lax">IPA (EA)</td>
    <td class="tg-0lax">*ov*   </td>
    <td class="tg-0lax">TARGET   </td>
    <td class="tg-0lax">ɑsɑt͡sʰ   </td>
  </tr>
  <tr>
    <td class="tg-0lax"></td>
    <td class="tg-0lax">Gloss</td>
    <td class="tg-0lax">who   </td>
    <td class="tg-0lax">TARGET   </td>
    <td class="tg-0lax">said</td>
  </tr>
  <tr>
    <td class="tg-0lax"></td>
    <td class="tg-0lax">Translation</td>
    <td class="tg-0lax" colspan="3">*Who* said TARGET? </td>
  </tr>
  <tr>
    <td class="tg-0lax"></td>
    <td class="tg-0lax">Orthography</td>
    <td class="tg-0lax" colspan="3">Ո՞վ «TARGET»&nbsp;&nbsp;&nbsp;ըսաւ/ասաց։</td>
  </tr>
  <tr>
    <td class="tg-0lax">Answer</td>
    <td class="tg-0lax">IPA (WA)</td>
    <td class="tg-0lax">*mɑɾjɑmə*</td>
    <td class="tg-0lax">TARGET   </td>
    <td class="tg-0lax">əsɑv   </td>
  </tr>
  <tr>
    <td class="tg-0lax"></td>
    <td class="tg-0lax">IPA (EA)</td>
    <td class="tg-0lax">*mɑɾjɑmə*</td>
    <td class="tg-0lax">TARGET   </td>
    <td class="tg-0lax">ɑsɑt͡sʰ   </td>
  </tr>
  <tr>
    <td class="tg-0lax"></td>
    <td class="tg-0lax">Gloss</td>
    <td class="tg-0lax">Mariam   </td>
    <td class="tg-0lax">TARGET</td>
    <td class="tg-0lax">said</td>
  </tr>
  <tr>
    <td class="tg-0lax"></td>
    <td class="tg-0lax">Translation</td>
    <td class="tg-0lax" colspan="3">*Mariam* said TARGET.</td>
  </tr>
  <tr>
    <td class="tg-0lax"></td>
    <td class="tg-0lax">Orthography</td>
    <td class="tg-0lax" colspan="3">Մարիամը «TARGET»&nbsp;&nbsp;&nbsp;ըսաւ/ասաց։</td>
  </tr>
</tbody>
</table>

<table class="tg">
<thead>
  <tr>
    <th class="tg-0lax">Type</th>
    <th class="tg-0lax"></th>
    <th class="tg-0lax" colspan="3">&nbsp;&nbsp;&nbsp;<br>&nbsp;&nbsp;&nbsp;Object focus dialogue</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0lax">Question</td>
    <td class="tg-0lax">IPA (WA)</td>
    <td class="tg-0lax">mɑɾjɑmə   </td>
    <td class="tg-0lax">*int͡ʃ*</td>
    <td class="tg-0lax">əsɑv   </td>
  </tr>
  <tr>
    <td class="tg-0lax"></td>
    <td class="tg-0lax">IPA (EA)</td>
    <td class="tg-0lax">mɑɾjɑmə   </td>
    <td class="tg-0lax">*int͡ʃʰ*</td>
    <td class="tg-0lax">ɑsɑt͡sʰ   </td>
  </tr>
  <tr>
    <td class="tg-0lax"></td>
    <td class="tg-0lax">Gloss</td>
    <td class="tg-0lax">Mariam   </td>
    <td class="tg-0lax">what</td>
    <td class="tg-0lax">said</td>
  </tr>
  <tr>
    <td class="tg-0lax"></td>
    <td class="tg-0lax">Translation</td>
    <td class="tg-0lax" colspan="3">*What* did Mariam say?</td>
  </tr>
  <tr>
    <td class="tg-0lax"></td>
    <td class="tg-0lax">Orthography</td>
    <td class="tg-0lax" colspan="3">Մարիամը ի՞նչ&nbsp;&nbsp;&nbsp;ըսաւ/ասաց։</td>
  </tr>
  <tr>
    <td class="tg-0lax">Answer</td>
    <td class="tg-0lax">IPA (WA)</td>
    <td class="tg-0lax">mɑɾjɑmə   </td>
    <td class="tg-0lax">*TARGET*   </td>
    <td class="tg-0lax">əsɑv   </td>
  </tr>
  <tr>
    <td class="tg-0lax"></td>
    <td class="tg-0lax">IPA (EA)</td>
    <td class="tg-0lax">mɑɾjɑmə   </td>
    <td class="tg-0lax">*TARGET*   </td>
    <td class="tg-0lax">ɑsɑt͡sʰ   </td>
  </tr>
  <tr>
    <td class="tg-0lax"></td>
    <td class="tg-0lax">Gloss</td>
    <td class="tg-0lax">Mariam   </td>
    <td class="tg-0lax">TARGET</td>
    <td class="tg-0lax">said</td>
  </tr>
  <tr>
    <td class="tg-0lax"></td>
    <td class="tg-0lax">Translation</td>
    <td class="tg-0lax" colspan="3">Mariam said *TARGET*.</td>
  </tr>
  <tr>
    <td class="tg-0lax"></td>
    <td class="tg-0lax">Orthography</td>
    <td class="tg-0lax" colspan="3">Մարիամը «TARGET»&nbsp;&nbsp;&nbsp;ըսաւ/ասաց։</td>
  </tr>
</tbody>
</table>

<table class="tg">
<thead>
  <tr>
    <th class="tg-0lax">Type</th>
    <th class="tg-0lax"></th>
    <th class="tg-0lax" colspan="3">&nbsp;&nbsp;&nbsp;<br>&nbsp;&nbsp;&nbsp;Verb focus dialogue</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0lax">Question</td>
    <td class="tg-0lax">IPA (WA)</td>
    <td class="tg-0lax">mɑɾjɑmə   </td>
    <td class="tg-0lax">TARGET   </td>
    <td class="tg-0lax">*ɡɑɾtɑt͡s*</td>
  </tr>
  <tr>
    <td class="tg-0lax"></td>
    <td class="tg-0lax">IPA (EA)</td>
    <td class="tg-0lax">mɑɾjɑmə   </td>
    <td class="tg-0lax">TARGET   </td>
    <td class="tg-0lax">*kɑɾtʰɑt͡sʰ*</td>
  </tr>
  <tr>
    <td class="tg-0lax"></td>
    <td class="tg-0lax">Gloss</td>
    <td class="tg-0lax">Mariam</td>
    <td class="tg-0lax">TARGET   </td>
    <td class="tg-0lax">read</td>
  </tr>
  <tr>
    <td class="tg-0lax"></td>
    <td class="tg-0lax">Translation</td>
    <td class="tg-0lax" colspan="3">Did Mariam *read* TARGET?</td>
  </tr>
  <tr>
    <td class="tg-0lax"></td>
    <td class="tg-0lax">Orthography</td>
    <td class="tg-0lax" colspan="3">Մարիամը «TARGET»&nbsp;&nbsp;&nbsp;կարդա՞ց։</td>
  </tr>
  <tr>
    <td class="tg-0lax">Interjection</td>
    <td class="tg-0lax">IPA (WA)</td>
    <td class="tg-0lax">vot͡ʃ</td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
  </tr>
  <tr>
    <td class="tg-0lax"></td>
    <td class="tg-0lax">IPA (EA)</td>
    <td class="tg-0lax">vot͡ʃʰ</td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
  </tr>
  <tr>
    <td class="tg-0lax"></td>
    <td class="tg-0lax">Gloss</td>
    <td class="tg-0lax">no</td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
  </tr>
  <tr>
    <td class="tg-0lax"></td>
    <td class="tg-0lax">Translation</td>
    <td class="tg-0lax" colspan="3">No</td>
  </tr>
  <tr>
    <td class="tg-0lax"></td>
    <td class="tg-0lax">Orthography</td>
    <td class="tg-0lax" colspan="3">Ոչ</td>
  </tr>
  <tr>
    <td class="tg-0lax">Answer</td>
    <td class="tg-0lax">IPA (WA)</td>
    <td class="tg-0lax">mɑɾjɑmə   </td>
    <td class="tg-0lax">TARGET   </td>
    <td class="tg-0lax">*əsɑv*</td>
  </tr>
  <tr>
    <td class="tg-0lax"></td>
    <td class="tg-0lax">IPA (EA)</td>
    <td class="tg-0lax">mɑɾjɑmə   </td>
    <td class="tg-0lax">TARGET   </td>
    <td class="tg-0lax">*ɑsɑt͡sʰ*   </td>
  </tr>
  <tr>
    <td class="tg-0lax"></td>
    <td class="tg-0lax">Gloss</td>
    <td class="tg-0lax">Mariam   </td>
    <td class="tg-0lax">TARGET</td>
    <td class="tg-0lax">said</td>
  </tr>
  <tr>
    <td class="tg-0lax"></td>
    <td class="tg-0lax">Translation</td>
    <td class="tg-0lax" colspan="3">Mariam *said* TARGET.</td>
  </tr>
  <tr>
    <td class="tg-0lax"></td>
    <td class="tg-0lax">Orthography</td>
    <td class="tg-0lax" colspan="3">Մարիամը «TARGET»&nbsp;&nbsp;&nbsp;ըսաւ/ասաց</td>
  </tr>
  <tr>
    <td class="tg-0lax">Negation</td>
    <td class="tg-0lax">IPA (WA)</td>
    <td class="tg-0lax">t͡ʃəɡɑɾtɑt͡s</td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
  </tr>
  <tr>
    <td class="tg-0lax"></td>
    <td class="tg-0lax">IPA (EA)</td>
    <td class="tg-0lax">t͡ʃʰəkɑɾtʰɑt͡sʰ</td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
  </tr>
  <tr>
    <td class="tg-0lax"></td>
    <td class="tg-0lax">Gloss</td>
    <td class="tg-0lax">not.read</td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
  </tr>
  <tr>
    <td class="tg-0lax"></td>
    <td class="tg-0lax">Translation</td>
    <td class="tg-0lax" colspan="3">She didn't read.</td>
  </tr>
  <tr>
    <td class="tg-0lax"></td>
    <td class="tg-0lax">Orthography</td>
    <td class="tg-0lax" colspan="3">չկարդաց։</td>
  </tr>
</tbody>
</table>

In the typical case, each type of question and answer sentence had its own special intonational contour, summarized in the following table.

<table class="tg">
<thead>
  <tr>
    <th class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Focus type</span></th>
    <th class="tg-0lax" colspan="2"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Utterance</span></th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Question (q)</span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Answer (a)</span></td>
  </tr>
  <tr>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Subject focus (tS)</span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Pitch-rise on subject</span><br><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Post-focal deaccenting</span><br><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Final rise (WA)</span><br><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Final fall (EA)</span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Pitch-rise on subject</span><br><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Post-focal deaccenting</span><br><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Final fall</span></td>
  </tr>
  <tr>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Object focus (tO)</span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Pitch-rise on object</span><br><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Post-focal deaccenting</span><br><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Final rise (WA)</span><br><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Final fall (EA)</span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Pitch-rise on object</span><br><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Post-focal deaccenting</span><br><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Final fall</span></td>
  </tr>
  <tr>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Verb focus (tV)</span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Pitch-rise on verb = final rise</span><br><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Optional pre-focal deaccenting</span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Optional pitch-rise on verb</span><br><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Final fall</span></td>
  </tr>
</tbody>
</table>

## Stress type of target word
The TARGET word varies in its stress location. It has one of the following conditions.


| Stress type   (code) | Subcategory   | Example WA  | Example EA    | Orthography | Translation     |
|----------------------|---------------|-------------|---------------|-------------|-----------------|
| Final (s3)           |               | dɑni**ki**  | tɑni**kʰi**   | տանիքի      | of the roof     |
| Final (s3a)          | adverb        |             | suto**ɾen**   | սուտորեն    | falsely         |
| Penult (s2)          | ends in /-ə/  | ki**d͡ze**ɾə | ɡi**t͡se**ɾə   | գիծերը      | the lines       |
| Penult (s2s)         | ends in /-əs/ | bɑ**di**ʒəs | pɑ**ti**ʒəs   | պատիժս      | my punishment   |
| Penult (s2t)         | ends in /-ət/ | mɑ**di**dət | mɑ**ti**tət   | մատիտդ      | your punishment |
| Initial (s1o)        | ordinal       | **u**teɾoɾt | **u**tʰeɾoɾtʰ | ութերորդ    | eighth          |
| Initial (s1a)        | adverb        | **su**doɾen |               | սուտօրէն    | falsely         |

# Materials
Recordings were made with 19 speakers: 10 for Eastern Armenian (5 female, 5 male) and 9 for Western Armenian (5 female, 4 male). In terms of origin, the Eastern Armenian speakers were from Yerevan, Armenia, while the Western Armenian speakers were from Aleppo, Syria. All 19 speakers were living in Yerevan during the time of the recording.  Speaker metadata is in file speaker-metadata (in [Excel](speaker-metadata.xlsx) and [TSV](speaker-metadata.tsv) versions).


The participants were recorded reading the dialogues on a PowerPoint presentation. In our annotation, we broke up each dialogue into its component utterances (Q, A, I, N) using a [Praat script](https://www.acsu.buffalo.edu/~cdicanio/scripts/Sound_file_division.praat). Each utterance is found in the repository in the form of a sound file `.wav`, a Praat TextGrid `.TextGrid`, and a transcript file `.txt`. Data is in the [data](data) folder. 

We annotated the recordings with information on quality. Most recordings had little to no disfluencies or background noise. These are found in the [data-few-issues](data/data-few-issues). 

Some recorded examples however had such problems. Files were annotated with the symbol `_?` if they had a mild issue in [data-moderate-issues](data/data-moderate-issues), and `_0` if they had a severe issue in [data-severe-issues](data/data-severe-issues).  We list such problems:
* Mild or moderate issues:
  * focus-unclear: The intonation is ambiguous.
  * laughing: The participant is laughing.
  * noise-mild: There is mild background noise. 
  * pause-mild: There is a small felicitous pause in the middle of the sentence.
  * pause-noise-mild: There is both mild background noise and a small pause.
  * unclear-segments: A segment was pronounced unclearly. 
* Severe issues:
  * focus-wrong-intonation: The participant used the wrong intonation. 
  * noise-extreme: There is extreme background noise.
  * pause-extreme: There is a long infelicitous pause in the middle of the sentence.
  * pause-noise-extreme: There is both extreme noise and a long pause. 
  * not-template: The utterance was misread in a way that doesn't fit into our templates, such as omitting the subject.
  * stutter-or-missing-sound: The participant stuttered in speech or omitted a sound.
 
We provided forced alignments using for the data-few-issues recordings. See the [Alignments folder](alignments).

# Recommendations

The recordings can be used for different purposes. We plan on using them for work on intonation phonetics and forced alignment. For phonetic studies, recordings with no or moderate issues can be suitable. But recordings with severe issues are not ideal or recommended. But for forced alignment, the recordings with severe issues might still be useful as a way to prevent overfitting or accommodating noisy data. 

The transcript files `.txt` are to make forced alignment tasks easier. The pronunciation dictionaries for [Western Armenian](word-pronunciations-WA.tsv) and [Eastern Armenian](word-pronunciations-EA.tsv) are for forced alignment purposes. 
    
# License

The dataset is made available to the research community licensed under the [GNU General Public License v3.0](https://www.gnu.org/licenses/gpl-3.0.en.html). 
    
# Contact

Feel free to contact us at `hossep.dolatian@alumni.stonybrook.edu` if you have any questions or concerns. 
