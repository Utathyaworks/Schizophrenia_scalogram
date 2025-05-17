# Schizophrenia Detection from Electroencephalogram Signals Using Image Encoding and Wrapper-based Deep Feature Selection Approach
## 📌 Overview
This repository contains the implementation of a novel three-stage deep learning-based framework for detecting schizophrenia from EEG signals. The proposed method leverages image encoding, transfer learning, and a newly developed Average Subtraction Wrapper-based Feature Selection method to improve classification accuracy and reduce computational overhead.

## 🧠 About Schizophrenia
Schizophrenia is a severe mental disorder that affects perception, cognition, emotions, and behavior, impacting approximately 1% of the global population. EEG (Electroencephalogram) signals offer a non-invasive and high-temporal-resolution way to detect subtle abnormalities in brain activity, which is valuable for early and accurate schizophrenia detection.

## 🚀 Proposed Framework
The framework comprises the following three main stages:

### Image Encoding of EEG Signals
Raw EEG time-series signals are converted into scalogram images using Continuous Wavelet Transform (CWT) to retain both spatial and temporal characteristics of the data.

### Feature Extraction using Transfer Learning
Two pre-trained deep learning models (EfficientNetB3 and DenseNet169) are applied to extract deep features from the encoded images.

### Average Subtraction Wrapper-based Feature Selection
A novel feature selection method is introduced to eliminate redundant and non-informative features, improving model performance and generalization.

## 📊 Datasets Used
### Dataset 1: M.S.U EEG Dataset
Source: M.V. Lomonosov Moscow State University

Total Subjects: 84

Schizophrenia: 45

Healthy: 39

### Dataset 2: RepOD EEG Dataset

Total Subjects: 28

Schizophrenia: 14

Healthy: 14

## 🎯 Results
### Dataset	Accuracy (%)
M.S.U EEG	99.67
RepOD EEG	99.97


📁 Repository Structure
1. EEG_scalo_conversion_final.ipynb
Description: Converts raw EEG signals into scalogram images using continuous wavelet transforms.
Input: Multichannel EEG recordings.
Output: Sscalogram images.

2. eeg-5-20-training.ipynb
Description: Trains classification models using the generated scalogram images.
Models:
DenseNet / EfficientNet
Output: Trained deep learning models and classification results.

3. Schizophrenia_feature_selection.ipynb
Description: Performs feature selection using the ASBO (Adaptive Swarm-Based Optimization) algorithm.

#

The proposed framework outperformed state-of-the-art methods on both datasets.

## Collaborator: [Arghyasree Saha](https://github.com/arghyasree-saha)

## Supervisor: [Dr. Pawan Kumar Singh](https://scholar.google.co.in/citations?user=LctgJHoAAAAJ&hl=en)
