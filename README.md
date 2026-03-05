# Credit Risk Default Prediction

## Project Overview

This project builds a machine learning model to predict the probability that a borrower will default on a loan.

Credit default prediction is a critical problem for financial institutions because it helps lenders reduce financial losses and make informed lending decisions.

The objective of this project is to build a robust predictive pipeline that can identify high-risk borrowers before issuing loans.

---

## Business Problem

Banks need to decide whether a loan applicant is likely to repay the loan.

Incorrect decisions can result in:

• Financial losses due to defaults  
• Reduced profitability  
• Higher capital risk  

This project predicts **loan default risk using historical borrower data.**

---

## Machine Learning Objective

Predict:

Probability(Default = 1)


for each borrower.

The model can then be used to:

• approve / reject loans  
• adjust interest rates  
• set credit limits  

---

## Project Structure

The project follows a structured ML workflow.


### 00 — Business Understanding
Defines the credit default problem and modeling objective.

### 01 — Data Understanding & Leakage
Examines dataset structure and prevents target leakage.

### 02 — Exploratory Data Analysis (EDA)
Explores relationships between borrower attributes and default risk.

### 03 — Feature Engineering
Transforms variables and prepares data for modeling.

### 04 — Modeling
Builds machine learning models to predict default probability.

---

## Models Used

The following models were explored:

• Logistic Regression  
• Random Forest  
• Gradient Boosting Models  

Model performance was evaluated using:

• ROC-AUC  
• Precision / Recall  
• Confusion Matrix  

---

## Evaluation Metric

Primary metric used:

**ROC-AUC**

Reason:

Credit default prediction is an **imbalanced classification problem**, and ROC-AUC measures the model’s ability to distinguish defaulters from non-defaulters across thresholds.

---
## Model Performance

| Model | ROC-AUC | Notes |
|------|------|------|
| Logistic Regression | 0.748 | Interpretable baseline model used in credit risk |
| XGBoost | 0.765 | Captures nonlinear relationships and feature interactions |

XGBoost achieved the best ROC-AUC score and was selected as the final model for predicting credit default risk.

## Dataset

The dataset used in this project contains anonymized borrower information including:

• credit history  
• income details  
• loan attributes  
• repayment behavior  

⚠️ Dataset is not uploaded to this repository due to size and licensing restrictions.

---

## Tech Stack

Python

Libraries used:

• Pandas  
• NumPy  
• Scikit-learn  
• Matplotlib  
• Seaborn  
• XGBoost  
• LogisticRegression

---

## How to Run the Project

Clone the repository

git clone


Install dependencies


pip install -r requirements.txt


Open Jupyter Notebook and run notebooks sequentially.

---

## Author

Suraj Jha






