# Chord Melody Dataset
This dataset to dedicated to the relationship between chords &amp; melodies.  The intended use case of the data set is to train models capable of predicting melodies from chord progressions or vice versa.

# 
The dataset conforms to a strict format.  All songs are saved in [MUSIC_XML](http://www.musicxml.com/for-developers/)

### Each bar must contain:
* 2 chords
* all notes MUST be monophonic (i.e single note melodies)
* notes and or rests that sum to 4 beats (4/4 time)
* triplets are NOT supported!
* the maximum resolution supported is 16th notes

### How the dataset was created
The dataset was created scaning leadsheets via the OCR feature in the [SMARTSCORE SOFTWARE](http://www.musitek.com/smartscore-pro.html)

### Contributing to the dataset
Ideally each song/leadsheet will be transposed to 12keys. I have created a golang app that will validate that the xml format is correct [MusicXmlParser](https://github.com/shiehn/MusicXmlGoParser)

### How to use this dataset
In order to use this data set to make musical predictions you must first encode the data into a format consumable by machine learning algorithms.  You are welcome to use the tool I've created or of course roll your own.  The encoder I've created is a simple GoLang commandline tool that consumes the MusicXML format and outputs enoded data strings. [ENCODING TOOL](https://github.com/shiehn/MusicXmlGoParser) 

For ideas on how to format and feed this data into machine learning algorithms & frameworks please visit my blog [Signals & Sorcery Blog](https://medium.com/@stevehiehn) or my procedural music generation project [TrebleMaker.Ai](http://treblemaker.ai/)
