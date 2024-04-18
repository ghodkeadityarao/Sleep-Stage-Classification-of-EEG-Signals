# Sleep Stage Classification using EEG Signals: A Comparative Study

## Overview
Disturbances in sleep adversely affect sleep quality, which can trigger various sleep-related conditions. Sleep stage classification is a crucial step in addressing such issues. This repository conducts a comprehensive comparative study of machine learning techniques for classifying sleep stages using input features derived from EEG signals.

## Dataset
We utilize the publicly available Sleep - EDF dataset, which consists of EEG recordings. These recordings are divided into 30-second chunks, and a time-frequency matrix of the Pseudo Wigner-Ville Distribution (PWVD) is obtained for each chunk.

Link: https://www.physionet.org/content/sleep-edf/1.0.0/

## Feature Extraction
- The time-frequency matrix is partitioned into frequency sub-bands.
- Features are derived from grey-scale and binary conversions of the sub-band matrices.
- The features are used to construct a dataset, where the Rechtschaffen and Kales (R&K) based scores of the chunks form the target labels.

## Machine Learning Techniques
We explore the following machine learning algorithms for sleep stage classification:
- Multinomial Logistic Regression (MLR)
- K-Nearest Neighbors (KNN)
- Decision Tree Classifier (DTC)
- Random Forest Classifier (RFC)
- MultiLayer Perceptron Classifier (MLP)

## Results
After conducting the experimental study, the performance of each technique is evaluated. The Multilayer Perceptron Classifier (MLP) emerges as the top performer, achieving an accuracy of 93.11%.
