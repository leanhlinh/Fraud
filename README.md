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

Usage

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

Confusion Matrix, Classification Report

Evaluation on an imbalanced test set to simulate real-world deployment

🧠 Interpretability
Used SHAP (SHapley Additive exPlanations) for:

Global feature importance

Local explanations for individual predictions

Key drivers: amount, merchant_category, international_flag

🚀 Usage
bash
Copy
Edit
# Clone the repo
git clone https://github.com/yourusername/aus-fraud-detection.git
cd aus-fraud-detection

# Install dependencies
pip install -r requirements.txt
Run the notebooks in Google Colab or locally

Export models:

xgb_fraud_model.joblib

tabnet_fraud_model.zip

(Optional) Deploy as API with FastAPI (template included)

🏁 Results
XGBoost and TabNet both achieved strong fraud detection metrics

SHAP plots provided clear transparency — critical for regulatory compliance

Full results with metrics and visuals are in the results/ folder


🙏 Acknowledgements
Inspired by insights from ASIC and the Australian Government Fraud Reports

Powered by:

scikit-learn, XGBoost, PyTorch TabNet, SHAP

pandas, matplotlib, seaborn



