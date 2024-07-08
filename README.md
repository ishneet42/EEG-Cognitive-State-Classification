# EEG Cognitive State Classification

## Overview
This project focuses on the analysis of EEG data to classify different cognitive states using advanced deep learning techniques. The data is sourced from the [Mental Arithmetic Tasks Dataset](https://physionet.org/content/eegmat/1.0.0/) available at PhysioNet. The dataset is pre-cleaned and ready for use, allowing you to concentrate on model implementation and evaluation. For a detailed understanding of the dataset, please refer to the accompanying [research paper](https://www.mdpi.com/2306-5729/4/1/14).

## Objectives
The primary objectives of this project are to:
1. Implement and evaluate multiple deep learning models using the Python library MNE.
2. Document the analysis in a Jupyter Notebook and submit it via a GitHub repository link.

## Steps to Achieve It

### 1. Load the EEG Data
- Load the EEG dataset provided by PhysioNet.

### 2. Power Spectral Density (PSD) Analysis
- **Calculate the band-wise PSD for both states:** 
  - Rest (recording EEG dataset before mental arithmetic task).
  - Task (recording of EEG dataset during the mental arithmetic task).
- **Focus on the following frequency bands:**
  - Delta (1-4 Hz)
  - Theta (4-8 Hz)
  - Alpha (8-12 Hz)
  - Beta (12-30 Hz)
  - Gamma (30-100 Hz)
- **Compare the PSDs of the two states and summarize your findings.**

### 3. Deep Learning Classification
- **Extract relevant features from the cleaned data.**
- **Implement binary classification using any two different deep learning models:** 
  - EEGNet
  - TSception
  - (Optional: ViT, ATCNet, VAE)
- **Train and validate the models using the provided dataset.**
- **Evaluate the models using appropriate metrics:**
  - Accuracy
  - Precision
  - Recall
  - F1-score
- **Discuss the results.**

## Models Used
1. **EEGNet**
   - A compact convolutional network for EEG-based brain-computer interfaces.
2. **TSception**
   - A temporal and spatial convolutional network for EEG-based emotion recognition.

## Results
- The results of the models are evaluated based on accuracy, precision, recall, and F1-score.
- Comparative analysis of the models is documented in the Jupyter Notebook.
