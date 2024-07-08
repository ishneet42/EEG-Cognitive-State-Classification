# EEG Cognitive State Classification

## Overview
This project focuses on the analysis of EEG data to classify different cognitive states using advanced deep learning techniques. The data is sourced from the [Mental Arithmetic Tasks Dataset](https://physionet.org/content/eegmat/1.0.0/) available at PhysioNet. The dataset is pre-cleaned and ready for use, allowing you to concentrate on model implementation and evaluation. For a detailed understanding of the dataset, please refer to the accompanying [research paper](https://www.mdpi.com/2306-5729/4/1/14).

## Objectives
The primary objectives of this project are to:
1. Implement and evaluate multiple deep learning models using the Python library MNE.
2. Document the analysis in a Jupyter Notebook and submit it via a GitHub repository link.

## Steps Undertaken and Achievements

### 1. Data Loading
- **What was done:** Loaded the EEG dataset provided by PhysioNet.
- **Achievement:** Successfully imported and prepared the dataset for analysis.

### 2. Power Spectral Density (PSD) Analysis
- **What was done:** 
  - Calculated the band-wise PSD for both states:
    - Rest (recording EEG dataset before mental arithmetic task).
    - Task (recording of EEG dataset during the mental arithmetic task).
  - Focused on the following frequency bands:
    - Delta (1-4 Hz)
    - Theta (4-8 Hz)
    - Alpha (8-12 Hz)
    - Beta (12-30 Hz)
    - Gamma (30-100 Hz).
  - Compared the PSDs of the two states.
- **Achievement:** Conducted comprehensive frequency domain analysis and summarized findings regarding differences between cognitive states.

### 3. Deep Learning Classification
- **What was done:**
  - Extracted relevant features from the cleaned data.
  - Implemented binary classification using two different deep learning models:
    - EEGNet
    - TSception
  - Trained and validated the models using the provided dataset.
  - Evaluated the models using metrics:
    - Accuracy
    - Precision
    - Recall
    - F1-score.
  - Discussed the results.

## Models Used
1. **EEGNet**
   - A compact convolutional network for EEG-based brain-computer interfaces.
2. **TSception**
   - A temporal and spatial convolutional network for EEG-based emotion recognition.

### Analysis and Discussion:
- **Accuracy:** EEGNet achieves a significantly higher accuracy (91.78%) compared to TSception (80.78%). This indicates that EEGNet is better at correctly classifying cognitive states from EEG data in this dataset.
  
- **Precision:** Both models show good precision, with EEGNet slightly higher at 92.61% compared to TSception at 85.39%. This suggests that EEGNet produces fewer false positives in its predictions.
  
- **Recall:** EEGNet and TSception have similar recall scores (91.78% vs. 80.78%), indicating effective identification of true positive instances, though EEGNet performs better overall.
  
- **F1-score:** EEGNet's F1-score (91.69%) is higher than TSception's (79.73%), reflecting its better balance between precision and recall.

### Conclusion:
- **EEGNet** outperforms **TSception** across all evaluated metrics (accuracy, precision, recall, and F1-score). It demonstrates superior capability in classifying cognitive states from EEG data, likely due to its specific architecture tailored for EEG-based tasks like brain-computer interfaces.
  
- **TSception**, while showing respectable metrics, does not achieve the same level of performance as EEGNet in this context. Depending on specific application requirements or dataset characteristics, TSception could be further optimized or combined with other techniques for enhanced performance.

These results underline the importance of selecting appropriate deep learning models tailored to the specific characteristics of EEG data and the desired classification task.
