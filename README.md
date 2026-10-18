# BankSim Fraud Detection Using Machine Learning

This repository contains the Python notebook developed for the research project Predicting Fraudulent Transactions in Financial Payment Systems Using Machine Learning Algorithms.

## Dataset

The study uses the BankSim dataset, consisting of 594,643 simulated financial transactions, including 7,200 fraudulent transactions.

The compressed dataset is provided as bs140513_032310.zip.

## Machine Learning Models

The analysis compares Logistic Regression, Random Forest and XGBoost, with Gradient Boosting included as an additional benchmark.

Model evaluation includes precision, recall, F1-score, ROC-AUC, average precision and five-fold stratified cross-validation. Limited Random Forest hyperparameter optimisation was conducted using GridSearchCV.

SMOTE-based resampling was not implemented in this study.

## Reproducing the Analysis

Open the .ipynb notebook in Google Colab.

Select Runtime → Run all.

The notebook automatically downloads and extracts the BankSim dataset from this repository.

The notebook performs data preprocessing, model training and evaluation.

The experiments use a stratified 70:30 training and test split, with random_state=42.

## Research Findings

Random Forest achieved the highest hold-out F1-score (0.8433), recall (0.7986) and average precision (0.9136). Logistic Regression achieved the highest ROC-AUC (0.9976).

These results relate to the BankSim synthetic dataset and should not be interpreted as evidence of performance in live financial payment systems.
