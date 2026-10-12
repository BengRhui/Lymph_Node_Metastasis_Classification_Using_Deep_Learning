# Lymph Node Metastasis Classification Using Deep Learning

A deep learning project utilising the PatchCamelyon (PCam) dataset to classify histopathological lymph node tissue images based on the presence of metastatic tumour tissue. The project explores and compares a baseline Convolutional Neural Network (CNN) and a hybrid CNN-Bidirectional Long Short-Term Memory (CNN-BiLSTM) architecture, with hyperparameter optimisation to improve classification performance.

---

## System Architecture

The project applies deep learning techniques to histopathological image classification, incorporating systematic data preparation, model development, hyperparameter tuning, and performance evaluation.

- **Language:** Python
- **Domain:** Deep Learning, Medical Image Classification, Computer Vision
- **Dataset:** PatchCamelyon (PCam)
- **Data Preparation:** Class Distribution Analysis, Duplicate Detection, Data Leakage Verification, Normalisation, Colour Deconvolution, Data Augmentation
- **Models Implemented:** Vanilla Convolutional Neural Network (CNN), Hybrid CNN-BiLSTM
- **Hyperparameter Optimisation:** Random Search
- **Model Evaluation:** Decision Threshold Selection, Classification Metrics, Learning Curves, Comparative Performance Analysis

---

## Core Modules

### Module 1: Dataset Selection & Exploration

- **Dataset Acquisition:** Utilises the PCam dataset, which contains histopathological image patches for binary classification of metastatic tumour tissue.
- **Exploratory Data Analysis:** Examines class distribution and visually inspects positive and negative samples to understand the dataset characteristics.
- **Data Quality Verification:** Investigates missing and invalid values, tissue content, duplicate samples, and potential cross-split data leakage.

### Module 2: Data Preparation & Preprocessing

- **Dataset Preparation:** Performs stratified sampling of the training split and verifies the prepared dataset before model development.
- **Image Normalisation:** Computes normalisation statistics to standardise image inputs for model training.
- **Colour Deconvolution:** Applies colour deconvolution techniques to process histopathological images.
- **Data Augmentation:** Introduces image transformations to improve training diversity and support model generalisation.

### Module 3: Deep Learning Model Development

- **Baseline CNN:** Develops a vanilla Convolutional Neural Network to extract spatial features from histopathological images and classify metastatic tumour presence.
- **Hybrid CNN-BiLSTM:** Combines CNN-based image feature extraction with Bidirectional Long Short-Term Memory (BiLSTM) layers to investigate an alternative classification architecture.
- **Model Training:** Configures and trains both architectures under defined training settings, monitoring validation performance and learning curves.

### Module 4: Hyperparameter Optimisation

- **Search Space Definition:** Establishes the hyperparameters and candidate configurations for model optimisation.
- **Random Search:** Explores different hyperparameter combinations to identify promising configurations.
- **Model Retraining:** Retrains the optimised models using their selected hyperparameter configurations.
- **Hyperparameter Analysis:** Examines the influence of hyperparameter choices on model performance.

### Module 5: Model Evaluation & Selection

- **Decision Threshold Selection:** Determines an appropriate classification threshold based on validation results.
- **Performance Evaluation:** Assesses model performance using selected classification metrics.
- **Comparative Analysis:** Compares baseline and optimised models using evaluation results and learning curves.
- **Champion Model Selection:** Selects the best-performing model based on the defined evaluation criteria.
- **Final Test Evaluation:** Evaluates the selected champion model on the test set to assess its performance on unseen data.

---

## Documentation

The project report that documents the dataset selection, preprocessing methodology, model architectures, training procedures, 
hyperparameter optimisation, and experimental results, can be viewed [here]().
