# Diabetes Risk Classification and Exploratory Data Analysis

This project analyses a diabetes dataset containing approximately 100,000 patient records and builds a machine learning model to predict diabetes risk.

## Project Overview

The workflow includes:

* Data cleaning and validation
* Exploratory data analysis
* Analysis of clinical risk factors
* Random Forest classification
* ROC-AUC, F1 and recall evaluation
* Feature importance analysis
* K-means clustering
* SMOTE experimentation
* SparkR distributed processing experimentation

## Dataset

* Original records: **100,000**
* Records after cleaning: **99,861**

The dataset contains clinical and demographic variables including:

* Age
* BMI
* HbA1c level
* Blood glucose level
* Hypertension
* Smoking history
* Diabetes status

## Model Performance

The final Random Forest classifier achieved:

| Metric   |    Result |
| -------- | --------: |
| ROC-AUC  | **0.868** |
| F1 Score | **0.801** |
| Recall   | **0.667** |

## Machine Learning

A Random Forest classifier was trained using an 80/20 train-test split.

The model used 500 decision trees and was evaluated using:

* Confusion matrix
* Precision
* Recall
* F1 score
* ROC curve
* ROC-AUC
* Feature importance

## Exploratory Analysis

The analysis investigated relationships between diabetes status and clinical variables including HbA1c, blood glucose, BMI and hypertension.

K-means clustering was also explored to identify groups of patients with similar clinical characteristics.

## Technologies

* R
* Random Forest
* SparkR
* ggplot2
* tidyverse
* caret
* pROC
* SMOTE
* K-means clustering

## Repository Structure

```text
diabetes-risk-classification/
│
├── README.md
│
└── analysis/
    └── diabetes_analysis.Rmd
```

## Notes

SMOTE was explored as a class-balancing technique, but the final Random Forest model uses the cleaned original dataset.

The SparkR section is a separate distributed-processing experiment using rule-based diabetes classification rather than the Random Forest model.
