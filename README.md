# Parkinson's Disease Telemonitoring Data Analysis

## Overview

This repository contains R scripts for analyzing Parkinson's disease telemonitoring data. The dataset used is from the UCI Machine Learning Repository and includes various biometric measures and Unified Parkinson's Disease Rating Scale (UPDRS) scores.

## Dataset

The dataset is sourced from the following URL: [Parkinson's Disease Telemonitoring Dataset](https://archive.ics.uci.edu/ml/machine-learning-databases/parkinsons/telemonitoring/parkinsons_updrs.data)

## Files

- `parkinsons_updrs_analysis.R`: R script containing data preprocessing, exploratory data analysis, statistical tests, data transformation, machine learning model building, and performance evaluation.
- `README.md`: This README file providing an overview of the project.

## Key Operations and Analyses

1. **Data Loading and Preprocessing**: The dataset is loaded from the URL using `read.csv` and subjected to initial data cleaning and removal of unnecessary columns (`subject`).

2. **Exploratory Data Analysis (EDA)**:
   - Summary statistics of the dataset are obtained using `summary()`.
   - Histograms and Q-Q plots are generated to visualize the distribution of variables.
   - Outlier detection using Tukey's method and identification of highly correlated variables are performed.

3. **Data Transformation**:
   - Log transformation is applied to selected columns to address skewness.
   - Standardization of features is performed using z-score scaling.

4. **Correlation Analysis**:
   - Pearson correlation coefficients are calculated to assess relationships between variables.

5. **Machine Learning Models**:
   - Linear Regression, Decision Trees, and Support Vector Regression (SVR) models are built and evaluated for predicting UPDRS scores.
   - Hyperparameter tuning is performed using cross-validation and grid search.

6. **Ensemble Model**:
   - An ensemble model is created by combining individual models using bootstrap sampling.
   - Performance metrics (MSE, MAE, R-squared) are calculated for the ensemble model.

## Usage

1. Clone the repository to your local machine.
2. Ensure you have R and necessary packages installed (`ggplot2`, `caret`, `e1071`, `rpart`, `car`).
3. Run the `parkinsons_updrs_analysis.R` script in an R environment to execute the analysis.

## Conclusion

The analysis provides insights into the Parkinson's disease telemonitoring data, including data preprocessing, exploratory analysis, machine learning model building, and evaluation. The ensemble model shows promising performance in predicting UPDRS scores based on biometric measures.
