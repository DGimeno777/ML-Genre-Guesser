# ML-Genre-Guesser

## Intro/Purpose
This project is meant to test if the genre of a song can be identified by processing its characteristics. The idea is that a song will be run through a processing library then can be run through a model to identify the genre.

## Specs/Details
### Primary Language(s)
We'll be starting off with Python as the main ML language for modeling data as well as for processing songs (mp3 or equiv.) to create data to train our models off of. This is mainly because Python is the language I have experience in with ML but also because Python supports a large number of libraries and a sound processing library that looks promising for this project.

## Data
### Considered Data
In the beginning we'll only consider songs from 4 genres that have little overlap. To avoid errors, each song will come from a different artist
These preliminary genres are:
- Jazz
- Punk Rock
- Hip-hop/Rap
- Classical

### Data Characteristics to Account For
- Song length: Punk songs typically short while Classical typically longer)
- Metre/Looping of beats: Hip-hip/Rap will typically have a similar beat across the entirly song while Jazz will more often change 
- Variety of notes played(?): Punk is very consistent with song note choice while other genres typically branch out 
- Average space between played notes and if they're different
- Instruments played (not sure if this can be detected easily but would be a huge help)
- Consistency of note panning for stereo mixing(?)
- Time Signature: Jazz/Classical usually use more uncommon time signatures
- Tempo (how fast the music is played)
(More to come & apologies for any misuse of music terminology)

### Problems to Consider from Data
1. Song Age - If only songs from a certain time span are used then the created model may not be able to identify those of the same genre from another period
2. Subgenres & Mixed Genres - Songs can sometimes fit into a number of different genres (or even be a mix of multiple) which could either confuse the model or possibly create a need for the model to be able to identify multiple genres that a song contains

## Resources
### Code Libraries
- [Python Sound Processing Library](https://www.youtube.com/watch?v=0ALKGR0I5MA)
- [Signal DSP Text](http://greenteapress.com/thinkdsp/thinkdsp.pdf)

### Musical References
- [Elements of a Song](https://www.futurelearn.com/courses/songwriting/0/steps/5711)
- [Average Genre Tempos](https://music.stackexchange.com/questions/4525/list-of-average-genre-tempo-bpm-levels)
- [Music Theory-Centri Tempo Explanation](http://www2.siba.fi/muste1/index.php?id=102&la=en)

# Credits
- [This guide](https://machinelearningmastery.com/machine-learning-in-python-step-by-step/) for providing the basics of ML
