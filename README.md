Online Payment Fraud Detection

This project detects fraudulent online payment transactions using data analysis and machine learning. 
The goal is to identify fraudulent activity in real time and prevent financial loss for users and companies.

Objective

Analyze transaction patterns to understand fraud behavior.
Build machine learning models that can predict fraud.
Compare model performance using multiple evaluation metrics.
Handle highly imbalanced classes in real-world fraud datasets.

---

Dataset Overview

The dataset contains features such as:
Transaction type
Transaction amount
Old and new account balances
Sender and receiver balances
Fraud flag (0 = Not Fraud, 1 = Fraud)
Fraud cases are very rare, making this a highly imbalanced classification problem.

---

Steps Performed

1 Data Cleaning

Inspected column types and structure.
Checked for missing values.
Handled outliers.
Converted categorical features into numeric.

2️ Exploratory Data Analysis (EDA)

Visualized fraud vs non-fraud transactions.
Analyzed transaction type distribution.
Identified patterns:
Fraud cases typically involve high-value transactions.
Specific transaction types show higher fraud probability.

3️ Feature Engineering

Created new features (if used).
Scaled numeric variables for ML models.
Encoded transaction types.

4️ Handling Class Imbalance

Applied one or more:
SMOTE oversampling
Class weights in ML models
Random oversampling

5 Machine Learning Models

Trained and evaluated:
Logistic Regression
Random Forest
XGBoost 

6️ Evaluation Metrics


Accuracy
Precision
Recall
F1 Score
Recall is the most important metric, because failing to detect fraud is more harmful.

---

7 Best Performing Model

XGBoost 

Why?
Handles imbalanced data better.
Captures complex non-linear fraud patterns.
Lower false negatives than simple models.

---

8 Tech Stack

Python
Pandas
NumPy
Matplotlib / Seaborn
Scikit-Learn
