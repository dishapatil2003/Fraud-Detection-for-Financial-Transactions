# Fraud-Detection-for-Financial-Transactions

📌 Project Overview

This project aims to detect fraudulent financial transactions using Machine Learning techniques. The dataset contains over 6.3 million transactions with features such as transaction type, amount, and account balances. Fraud detection is critical for preventing financial losses and enhancing security.

✅ Objectives

Predict fraudulent transactions using machine learning models.

Identify key features that indicate fraud.

Handle imbalanced data using SMOTE.

Provide actionable insights for fraud prevention.

📂 Dataset

Rows: 6,362,620

Columns: 10

Key Features:

step: Time step in hours

type: Transaction type (CASH-IN, CASH-OUT, DEBIT, PAYMENT, TRANSFER)

amount: Transaction amount

oldbalanceOrg, newbalanceOrig: Sender’s balance before and after transaction

oldbalanceDest, newbalanceDest: Receiver’s balance before and after transaction

isFraud: Target variable (1 = Fraud, 0 = Not Fraud)

🛠 Technologies Used

Python

Pandas, NumPy – Data preprocessing

Seaborn, Matplotlib – Data visualization

Scikit-learn – Model building and evaluation

Imbalanced-learn (SMOTE) – Handle class imbalance

Random Forest – Primary model

(Optional) XGBoost / LightGBM for comparison

🔍 Approach

Data Cleaning: Removed irrelevant columns, encoded categorical features.

Exploratory Data Analysis (EDA):

Fraud vs Non-Fraud distribution

Transaction type analysis

Correlation heatmap

Feature Engineering:

Added balance_diff_orig and balance_diff_dest

Handle Imbalance:

Applied SMOTE to balance classes

Modeling:

Random Forest Classifier

Performance evaluation using F1-score, ROC-AUC

Business Insights:

Key fraud indicators identified

Prevention strategies recommended

📊 Model Performance

F1-score: ~0.92

ROC-AUC: ~0.95

Precision-Recall optimized for imbalanced data

📈 Key Insights

Fraud mainly occurs in TRANSFER and CASH-OUT transactions.

High-value transactions with sudden account balance drops are strong indicators of fraud.
