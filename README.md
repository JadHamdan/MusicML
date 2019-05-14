# MusicML
Exploring some of the many ways one can use music with machine learning, from classification to music generation.

## Music Classification:
In this repository, you can find multiple attempts at classifying music by genre using different machine learning algorithms. 
In "Feature Extraction + Classification", I preprocessed my audio data by extracting various features from the the audio signal of each song,  using the Librosa Python Library. These include Spectral Centroid, Zero Crossing Rate, Spectral Rolloff, etc. I then used algorithms from the sci-kit learn library as a first classificationa attempt (Random Forest, Support Vector Machine and others).

This first attempt yielded dissapoint results, leading me to trying a different approach. Using tht same python library, I extracted the "Mel-Spectrogram" from each audio file and treated the problem as an image classification task. I thus used a convolutional neural network to classify the extracted images leading to a much higher accuracy (see the Music Classification Using CNN directory).

## Music Generation:
Using ABC notation, a way of writing sheet music using simple ascii characters, I treated music generation as a text generation exercise. Hence, I trained a Long Short Term Network memory network in Keras with data from the Nottingham Music Database to generated simple yet aesthetically pleasing tunes.


### For more details, see the "Project Deliverable 3" pdf file as it explains every step of this project in depth. 
This project is part of the MAIS202 accelerated machine learning bootcamp, organized by the McGill AI Society
