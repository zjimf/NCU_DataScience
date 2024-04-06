# To Ensemble And Beyond

## Overview

This document details an experiment aimed at predicting gender within a dataset through sentiment analysis and various classifiers. The study assesses the performance of different data processing methods and machine learning models, with a focus on the impact of feature engineering on model performance.

## Introduction

The experiment employs a range of preprocessing methods and a stacking classifier combining decision trees, XGBoost, and logistic regression. The objective is to optimize prediction outcomes through ensemble learning strategies.

## Dataset

The dataset contains 423 records, encompassing variables like basic personal information, physiological characteristics, social behaviors, and self-expression modes. Key variables include gender, star sign, phone operating system, height, weight, sleepiness level, IQ, number of Facebook friends, daily YouTube usage, and a self-introduction text.

## Methodology

- **Preprocessing:**
  - Removal of outliers in features like height, weight, number of Facebook friends, and YouTube watch duration.
  - Imputation of missing values using mean for numerical features and mode for categorical features.
  - Application of One-Hot Encoding for categorical variables.
  - Utilization of TF-IDF for text data transformation.
  - Use of SMOTETomek for handling data imbalance.
- **Classifiers:**
  - Decision Tree, XGBoost, and Logistic Regression individually, and combined in a Stacking Classifier.
  - Evaluation of model performance through accuracy, F1 score, ROC AUC, and other metrics.

## Results

- The stacking model combining Decision Tree and XGBoost with Logistic Regression as the meta-model achieved the highest accuracy.
- Outlier removal, imputation, One-Hot Encoding, and TF-IDF transformation were essential in enhancing model performance.
- The Stacking Classifier approach demonstrated superior predictive performance across various evaluation metrics.

## Conclusion

Effective data preprocessing and the strategic use of ensemble learning significantly improved gender prediction accuracy. The study underscores the importance of feature engineering and model selection in machine learning tasks related to human behavior and characteristics.
