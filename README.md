# 🏦 Loan Approval Screening Using Machine Learning

A Machine Learning project developed as part of my **Learn Depth Internship** to predict whether a loan application is likely to be **Approved or Rejected** based on financial and employment-related information.

## 📌 Project Overview

The objective of this project is to build a classification model that can assist in screening loan applications using applicant-related features such as income, credit score, debt-to-income ratio, employment experience, loan amount, and previous defaults.

The project follows an end-to-end Machine Learning workflow:

**Data → Cleaning → EDA → Preprocessing → Model Training → Evaluation → Prediction**

## 🎯 Objectives

- Analyze loan applicant data
- Clean and preprocess the dataset
- Perform Exploratory Data Analysis (EDA)
- Train a Logistic Regression classification model
- Evaluate model performance using multiple metrics
- Analyze feature influence
- Predict loan approval for new applicants

## 📊 Dataset Features

| Feature | Description |
|---|---|
| `income_monthly` | Applicant's monthly income |
| `credit_score` | Applicant's credit score |
| `debt_to_income` | Debt-to-income ratio |
| `employment_years` | Years of employment |
| `loan_amount` | Requested loan amount |
| `prior_defaults` | Number of previous loan defaults |
| `target` | Loan decision: 0 = Rejected, 1 = Approved |

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Google Colab

## 🤖 Machine Learning Model

**Algorithm:** Logistic Regression

Before training, the numerical features were standardized using `StandardScaler`.

The dataset was divided into:

- **80% Training Data**
- **20% Testing Data**

The model was evaluated using:

- Accuracy
- Precision
- Recall
- F1 Score
- ROC-AUC
- Confusion Matrix
- ROC Curve

## 📈 Model Performance

| Metric | Score |
|---|---:|
| Accuracy | 70.50% |
| Precision | 68.81% |
| Recall | 75.00% |
| F1 Score | 71.77% |
| ROC-AUC | 78.23% |

The model achieved an ROC-AUC of **0.7823**, showing a reasonable ability to distinguish between approved and rejected loan applications.

## 🔍 Project Workflow

1. Dataset Loading
2. Data Inspection
3. Data Cleaning
4. Exploratory Data Analysis
5. Feature and Target Separation
6. Train-Test Split
7. Feature Scaling
8. Logistic Regression Training
9. Model Prediction
10. Model Evaluation
11. Confusion Matrix Analysis
12. ROC Curve Analysis
13. Feature Influence Analysis
14. New Applicant Prediction

## 📌 Sample Prediction

The trained model was also tested on new applicant data to predict:

- Loan approval/rejection
- Approval probability

## 📂 Project Structure

```text
Loan-Approval-Screening/
│
├── loan_approval_screening.ipynb
├── dataset_02_loan_approval_screening.csv
└── README.md
