# chord-melody-dataset
This dataset to dedicated to the relation ship between chords &amp; melodies

# 
The dataset conforms to a strict format.  All songs are saved in [MUSIC_XML](http://www.musicxml.com/for-developers/)

###Each bar must contain:
* 2 chords
* all notes MUST be monophonic (i.e single note melodies)
* notes and or rests that sum to 4 beats (4/4 time)
* triplets are NOT supported!
* the maximum resolution supported is 16th notes

###How the dataset was created
The dataset was created scaning leadsheets via the OCR feature in the [SMARTSCORE SOFTWARE](http://www.musitek.com/smartscore-pro.html)

###Contributing to the dataset
Ideally each song/leadsheet will be transposed to 12keys. I have created a golang app that will validate that the xml format is correct [MusicXmlParser](https://github.com/shiehn/MusicXmlGoParser)

###How to use this dataset
For ideas on how to format and feed this data into machine learning algorithms & frameworks please visit my blog [Signals & Sorcery Blog](https://medium.com/@stevehiehn) or my procedural music generation project [Signals & Sorcery](http://signalsandsorcery.com/)