👤 Author
Anh Linh Le
📧 leanhlinh2808@gmail.com
📍 Melbourne, Australia

Australian Transaction Fraud Detection
End-to-End Machine Learning Pipeline for Credit Card Fraud in Australia

Detect and understand fraudulent transactions using advanced models like XGBoost and TabNet, enriched with SHAP interpretability, deployment-ready structure, and fully synthetic data reflecting Australian fraud patterns.

📚 Table of Contents
Project Overview

Data

EDA & Feature Engineering

Modeling

Evaluation

Interpretability


Results

Acknowledgements


🔍 Project Overview
This project presents an end-to-end machine learning pipeline tailored for fraud detection in Australian financial transactions. It includes:

Synthetic dataset informed by Australian fraud trends and ASIC reports

Exploratory Data Analysis (EDA)

Feature engineering (risk-based features)

Class imbalance handling (SMOTE)

Training & evaluation of advanced ML models (XGBoost, TabNet)

Model explainability with SHAP

Deployment-ready code with optional FastAPI integration

📦 Data
Source: Synthetic, based on Australian fraud trends and ASIC reports

Features Include:

amount, state, merchant_category, card_present, international_flag, transaction_time

Engineered: high_amount_flag, risky_merchant, night_transaction

Target: is_fraud (binary)

📊 EDA & Feature Engineering
Analyzed fraud rates across amount bands, merchant types, states, and transaction time

![image](https://github.com/user-attachments/assets/1655b258-1d13-4330-99ac-c126f81f93e1)

![image](https://github.com/user-attachments/assets/ec70514f-25ea-4a0e-9171-f07813adb314)

![image](https://github.com/user-attachments/assets/e4db5ed1-b8c8-4384-ba3f-5a69e41577bd)

![image](https://github.com/user-attachments/assets/f5911b3c-af52-417a-8a53-36776bfa1656)

![image](https://github.com/user-attachments/assets/1737fc2f-2a32-4260-bb25-d098631708bd)


Engineered domain-relevant features like:

high_amount_flag

risky_merchant

night_transaction

Applied one-hot encoding for categorical features

🤖 Modeling
Class Imbalance Handling: SMOTE oversampling

Models Used:

🏆 XGBoost: Gradient-boosted decision trees

🔬 TabNet: Deep learning for tabular data

Hyperparameter tuning via cross-validation

📈 Evaluation
Metrics:

ROC AUC, Precision-Recall AUC
![image](https://github.com/user-attachments/assets/6e399264-d841-486b-ab5b-561b4eec0a84)

![image](https://github.com/user-attachments/assets/b28fd6ff-83e6-4536-aa85-357cf77aec7c)


Confusion Matrix, Classification Report

![image](https://github.com/user-attachments/assets/90d7a1b4-28af-416d-8412-bf21575fdcfd)


Evaluation on an imbalanced test set to simulate real-world deployment

🧠 Interpretability
Used SHAP (SHapley Additive exPlanations) for:

Global feature importance

Local explanations for individual predictions

Key drivers: amount, merchant_category, international_flag


🏁 Results
XGBoost and TabNet both achieved strong fraud detection metrics

![image](https://github.com/user-attachments/assets/3fd1b641-efab-47e0-9294-7bccad47cfae)


SHAP plots provided clear transparency — critical for regulatory compliance

![image](https://github.com/user-attachments/assets/e65155e5-4e8b-4075-b909-f7e2d0e8651c)

![image](https://github.com/user-attachments/assets/d14014e6-cb6d-4ed0-84f0-9258726e60cf)



Full results with metrics and visuals are in the results/ folder


🙏 Acknowledgements
Inspired by insights from ASIC and the Australian Government Fraud Reports

Powered by:

scikit-learn, XGBoost, PyTorch TabNet, SHAP

pandas, matplotlib, seaborn



