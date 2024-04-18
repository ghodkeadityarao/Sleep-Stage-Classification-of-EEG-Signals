# Sleep Stage Classification using EEG Signals: A Comparative Study

## Overview
Disturbances in sleep adversely affect sleep quality, which can trigger various sleep-related conditions. Sleep stage classification is a crucial step in addressing such issues. This repository conducts a comprehensive comparative study of machine learning techniques for classifying sleep stages using input features derived from EEG signals.

![image](https://github.com/ghodkeadityarao/Sleep-Stage-Classification-of-EEG-Signals/assets/99025242/e12bb42e-8488-4d29-bdc7-896abe7873e6)

## Dataset
We utilize the publicly available Sleep - EDF dataset, which consists of EEG recordings. These recordings are divided into 30-second chunks, and a time-frequency matrix of the Pseudo Wigner-Ville Distribution (PWVD) is obtained for each chunk.

Link: https://www.physionet.org/content/sleep-edf/1.0.0/

## Feature Extraction
- The time-frequency matrix is partitioned into frequency sub-bands.
![image](https://github.com/ghodkeadityarao/Sleep-Stage-Classification-of-EEG-Signals/assets/99025242/0b9cc1a3-18b9-4350-8087-7d53ae961ea4)
  
- Features are derived from grey-scale and binary conversions of the sub-band matrices.
![image](https://github.com/ghodkeadityarao/Sleep-Stage-Classification-of-EEG-Signals/assets/99025242/41d45694-abff-49c5-bf6e-74757c25552e)

![image](https://github.com/ghodkeadityarao/Sleep-Stage-Classification-of-EEG-Signals/assets/99025242/8f3c6e69-4737-47d3-9afc-2e86a6ea6f29)


- The features are used to construct a dataset, where the Rechtschaffen and Kales (R&K) based scores of the chunks form the target labels.

## Machine Learning Techniques
We explore the following machine learning algorithms for sleep stage classification:
- Multinomial Logistic Regression (MLR)
- K-Nearest Neighbors (KNN)
- Decision Tree Classifier (DTC)
- Random Forest Classifier (RFC)
- MultiLayer Perceptron Classifier (MLP)

![image](https://github.com/ghodkeadityarao/Sleep-Stage-Classification-of-EEG-Signals/assets/99025242/7b98abef-dbd9-47ee-9b60-0680cf9190b6)


## Results
After conducting the experimental study, the performance of each technique is evaluated. The Multilayer Perceptron Classifier (MLP) emerges as the top performer, achieving an accuracy of 93.11%.

![image](https://github.com/ghodkeadityarao/Sleep-Stage-Classification-of-EEG-Signals/assets/99025242/a7710523-31df-45a2-8967-4b1605d4d99b)

