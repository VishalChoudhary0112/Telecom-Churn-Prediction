# Telecom Churn Prediction

## Overview

This project focuses on predicting customer churn in the telecom sector, where churn rates significantly impact revenue and customer acquisition costs. Using various machine learning techniques and statistical analysis, this project aims to build a robust predictive model that helps telecom companies identify customers likely to churn and take preventive measures.

## Project Resources

This repository includes key resources that summarize the analysis, methodology, and outcomes of the project:

- **Uploaded Files:**: [Raw datasets used for analysis](https://github.com/VishalChoudhary0112/Telecom-Churn-Prediction/blob/main/Telecom%20Churn/cell2cell.csv)
- **Business Presentation Report:**: [Detailed report outlining the business understanding, model findings, and strategic recommendations](https://github.com/VishalChoudhary0112/Telecom-Churn-Prediction/blob/main/Telecom%20Churn/Presentation_report.pdf)
- **Detailed Project Report:**: [Extensive report covering all aspects of the project including methodology, code, and insights](https://github.com/VishalChoudhary0112/Telecom-Churn-Prediction/blob/main/Telecom%20Churn/Telecom_churn_report.pdf)


## Table of Contents

- [Project Background](#project-background)
- [Dataset Information](#dataset-information)
- [Data Preprocessing](#data-preprocessing)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Model Building & Evaluation](#model-building--evaluation)
- [Best Model Summary](#best-model-summary)
- [Limitations](#limitations)
- [Conclusion](#conclusion)
- [Contributors](#contributors)
- [License](#license)

## Project Background

Churn prediction is a crucial challenge for telecom companies, given the high cost of acquiring new customers compared to retaining existing ones. The goal is to identify at-risk customers using their historical behavior and profile data.

### Objectives

- Identify key factors contributing to customer churn.
- Build and compare multiple ML classification models.
- Use feature engineering and statistical testing to improve prediction performance.
- Recommend the most effective model and strategy.

## Dataset Information

- **Source**: Kaggle
- **Records**: 51,047
- **Features**: 58 total, 21 categorical
- **Target Variable**: `Churn`
- **Redundant Features Dropped**: Customer ID, Service Area

## Data Preprocessing

- **Null Handling**: Imputation using KNN for `Age`, `Marital Status`; dropping columns like `Handset Price` with >50% nulls.
- **Outlier Detection**: Boxplots and transformation using Yeo-Johnson.
- **Class Imbalance**: Handled using SMOTE.
- **Multicollinearity**: Detected and mitigated.
- **Statistical Tests**: Kruskal-Wallis for dependency check, Chi-Square for categorical independence.

## Exploratory Data Analysis

- High churn among users with internet-enabled phones.
- Credit card holders showed higher churn tendency.
- Age, service usage, and web capability were strong indicators.
- EDA helped in reducing dimensionality and improving feature significance.

## Model Building & Evaluation

A variety of models were built and evaluated:

| Model | Accuracy | 
|-------|----------|
| XGBoost | 70% |
| Naive Bayes | 0.68% |
| **Stack Model** | **71%** | 

## Best Model Summary

- **Stacking Classifier** outperformed others with the highest accuracy of 71%
- The model's performance insights are crucial for implementing effective customer retention strategies.

## Limitations
- Class imbalance was a major challenge despite using SMOTE.
- Statistical assumptions were not met (non-normal data).
- Lack of domain expertise limits some insights and feature engineering steps.



