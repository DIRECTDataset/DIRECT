# DIRECT - DIalogue-based REading Comprehension Tutoring Dataset

### Description
DIRECT is a DIalogue-based REading Comprehension Tutoring dataset, in which the tutor asks questions and gives feedback, while student answers can be correct or incorrect. Similar to a tutor in a real one-on-one tutoring situation, this dataset also includes a chat about a given passage. Other annotations, including key sentences and student answer assessment labels.

The DIRECT dataset adopts the RACE dataset reading worksheets to simulate tutoring conversations. We chose RACE because it is a collection of reading comprehension exercises constructed by human experts for practical teaching ([Lai et al., 2017](https://arxiv.org/abs/1704.04683)). We focused on the RACE-M subset for middle school examinations.
 
Here we release the test/dev and partial training sets of DIRECT Dataset. It can be used along with or without the RACE corpus for following research tasks:
1) Dialogue-based reading comprehension tutoring task 
2) Question generation task 
3) Feedback generation task 
4) Student answer assessment tasks (NLI task)
5) Dialogue generation task


### Paper
J.X. Huang, Y. Lee and O.W. Kwon, "[DIRECT: Toward Dialogue-Based Reading Comprehension Tutoring](http://doi.org/10.1109/ACCESS.2022.3233224)," in IEEE Access, doi: 10.1109/ACCESS.2022.3233224.


### Notes
1. DIRECT dataset is available for non-commercial research purpose only.
2. The dialogues are developed based on RACE Dataset. 
3. You agree not to reproduce, duplicate, copy, sell, trade, resell or exploit for any commercial purpose, any portion of the contexts and any portion of derived data.
4. We reserve the right to terminate your access to the DIRECT Dataset at any time.


### Data Usage
One dialogue of DIRECT is correspondent to one passage in RACE.
- file_id: it is an article id, correspond to the passage id in RACE dataset.
- dialogue: a multi-tun dialogue, based on the correspond article and exercise in RACE dataset.
- speaker: the role of the speakers involved in the conversation, can be “tutor” or “student”.
- text: utterance of the speaker.
- type: the type of the tutor utterance, can be one of “Question”, “Feedback”, and “Chat”. “Question” is natural language question constructed based on the exercise in RACE dataset.
- label: the label of the student utterance, can be “correct”, “incorrect”, or none. None is for “Chat” type tutor utterance.
- key_sentence: the sentence in the corresponding passage of RACE, related with the given question or feedback of tutor utterance. 


### Dataset download
Part of the dataset is available at [ETRI Nanum](https://nanum.etri.re.kr/share/jxhuang/DIRECT?lang=en_US) website. You need to register and login first for download.


