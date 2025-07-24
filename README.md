#                                      Fraud Detection System

This repository contains a machine learning pipeline for detecting fraudulent transactions using two real-world datasets. It combines e-commerce and credit card transaction data with IP geolocation information to build accurate and explainable fraud detection models.

##  Problem Statement

Financial fraud leads to billions in losses globally. This project aims to build a robust fraud detection system that identifies fraudulent transactions while minimizing false positives, using both behavioral and geolocation data.

##  Project Structure

├── data/ # Raw and processed datasets (not pushed to Git)
├── notebooks/ # Jupyter notebooks for EDA and modeling
├── src/ # Core source code (data prep, modeling, etc.)
├── scripts/ # Utility scripts or CLI tools
├── tests/ # Unit tests
├── configs/ # Config files (e.g., model params)
├── requirements.txt # Python dependencies
├── README.md # Project documentation
└── .gitignore

markdown
Copy code

##  Features

- Cleans and preprocesses transaction data
- Maps IP addresses to countries
- Extracts time and frequency-based features
- Handles class imbalance with SMOTE
- Scales and encodes features
- Trains and evaluates fraud detection models
- Uses explainability techniques for model insights

##  Requirements

Install dependencies with:

```bash
pip install -r requirements.txt
Datasets
    Fraud_Data.csv: E-commerce transaction data
    IpAddress_to_Country.csv: Maps IP ranges to countries
    creditcard.csv: Anonymized bank transaction data

Note: Datasets are stored locally in /data and are ignored by Git.

Models
Models are built using:
Logistic Regression
Random Forest
XGBoost
Evaluation includes metrics like precision, recall, F1, ROC-AUC, and confusion matrix.