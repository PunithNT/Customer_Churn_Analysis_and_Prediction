# Customer_Churn_Analysis_and_Prediction
This repository contains a comprehensive pipeline for analyzing and predicting customer churn within the telecommunications industry.

# Project Overview

# Objective
This project is divided into two parts:
1. Exploratory Data Analysis (EDA):
  o Investigate the dataset for patterns, correlations, and anomalies.
  o Utilize Python's classic EDA libraries (NumPy, Pandas, Seaborn, Matplotlib) and automated tools (Pandas Profiling, SweetViz).
  o Prepare the dataset for predictive modeling by handling missing values, outliers, and transformations.

2. Predictive Modeling:
  o Build classification models (Na�ve Bayes, Logistic Regression, Random Forest, XGBoost) to predict customer churn.
  o Evaluate models on two datasets:
    * Original dataset.
    * Dataset balanced using SMOTE (Synthetic Minority Over-sampling Technique).
  o Assess model performance using metrics (Accuracy, Precision, Recall, F1-Score), emphasizing Recall.

# Dataset
The dataset consists of 7043 rows and 21 columns. It includes customer demographic details, service usage, billing information, and a target variable indicating churn status (Churn).
Features:
* Categorical Features (17): e.g., gender, InternetService, Contract, etc.
* Numerical Features (3): tenure, MonthlyCharges, TotalCharges.
* Target Feature (1): Churn (indicating if a customer churned or not).

# Features of the Project
1. Data Cleaning:
  o Handled missing and invalid data in columns like TotalCharges.
  o Converted all categorical columns to numeric values.

2. EDA:
  o Visualized feature distributions and dependencies.
  o Generated detailed reports using SweetViz and Pandas Profiling.
  o Explored correlations among numeric features and churn dependencies.

3. Modeling Pipeline:
  o Balanced the dataset using SMOTE.
  o Trained and evaluated multiple models using standardized metrics.
  o Tuned hyperparameters for the Random Forest model.

4. Visualization:
  o Boxplots for numeric features.
  o Heatmaps to study correlations.
  o Countplots for churn distribution across categorical variables.

# Usage

# Requirements
  * Python 3.7 or higher
  * Install the required libraries:
    bash

# Sample libraries:
o pandas
o numpy
o sweetviz
o seaborn
o matplotlib
o scikit-learn
o imbalanced-learn
o xgboost

# Run the Analysis
1. Place the dataset (telco_customer_churn.csv) in the data/ directory.
2. Open and execute the Jupyter notebooks:
  o EDA and Visualization: eda_analysis.ipynb
  o Modeling and Evaluation: modeling_pipeline.ipynb

# Output
* HTML-based SweetViz report: reports/SweetViz_Comparison.html.
* Evaluation metrics for each model.

# Results
Key Findings
* Strong correlation between churn and features like Contract, PaymentMethod, and MonthlyCharges.
* Customers on month-to-month contracts are more likely to churn compared to longer-term contracts.

# Limitations
1. Imbalanced dataset before applying SMOTE.
2. Lack of additional demographic or behavioral data.
3. Some categorical variables were reduced to numeric labels, potentially losing context.

# Future Work
* Experiment with additional feature engineering techniques.
* Implement advanced models like Neural Networks.
* Incorporate feature importance into decision-making.

# License
This project is developed as part of coursework and is for educational purposes only.

Feel free to clone this repository and contribute by raising issues or submitting pull requests!
