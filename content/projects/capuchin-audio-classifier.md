--- 
title: "Capuchin Bird Audio Classifier" 
description: "Deep learning model for detecting Capuchin bird calls in forest recordings" 
dateString: Mar 2021 - Jun 2021 
draft: false 
tags: ["TensorFlow", "Audio Processing", "Deep Learning", "Spectrograms", "CNN", "Signal Processing", "Wildlife Conservation", "Python", "Audio Classification", "Machine Learning"] 
showToc: false 
weight: 305
cover:
   image: "projects/capuchin-audio-classifier/yamnet_animation (2).gif" 
---

<userStyle>Normal</userStyle>

##### 🔗 [GitHub](https://github.com/faseehahmed26/CapuchinClassifier)
##### 🔗 [Dataset](https://www.kaggle.com/code/duanboomer/capuchin-bird-audio-classification)

## Description

* Developed a deep learning audio classification system that detects Capuchin bird calls in rainforest recordings, achieving 100% recall and precision on validation data after only 4 training epochs.

* Implemented end-to-end audio processing pipeline using TensorFlow and TensorFlow IO, handling everything from raw WAV/MP3 files to model-ready spectrograms.

* Created custom audio preprocessing functions to resample audio from 44.1kHz to 16kHz, normalize amplitudes, and generate time-frequency spectrograms using Short-Time Fourier Transform (STFT).

* Engineered an efficient data loading workflow for handling variable-length audio files by padding shorter clips and creating equal-length windows (48,000 samples) across longer recordings.

* Built and trained a CNN model architecture with two convolutional layers, max pooling, and dense layers optimized for spectrogram pattern recognition in audio signals.

* Designed custom forest recording parsing functions to analyze extended MP3 audio files by splitting them into overlapping windows and making sequential predictions.

* Implemented post-processing algorithms using itertools to group consecutive positive detections, effectively counting distinct Capuchin calls in continuous forest recordings.

* Created a scalable system that processes complete forest audio recordings to accurately count Capuchin bird calls, enabling wildlife conservation monitoring and research.

* Optimized the model to minimize false positives and achieved near-perfect accuracy in distinguishing Capuchin calls from other rainforest sounds in noisy environments.

* Generated CSV outputs with processed results for visualization and analysis, along with a saved model artifact for deployment in field research applications.