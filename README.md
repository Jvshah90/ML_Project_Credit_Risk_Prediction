# ML_Project_Credit_Risk_Prediction

📌 Project Overview

This project predicts whether a loan applicant is likely to default on a loan using Machine Learning. It follows an end-to-end data science workflow, including data preprocessing, exploratory data analysis (EDA), feature engineering, model building, hyperparameter tuning, and evaluation.

The goal is to help financial institutions make data-driven lending decisions and reduce credit risk.

🚀 Features
Data cleaning and preprocessing
Handling missing values and duplicates
Outlier detection and removal
Business rule validation
Exploratory Data Analysis (EDA)
Feature Engineering
Feature Selection
Multicollinearity analysis using VIF
Categorical Encoding
Feature Scaling
Class imbalance handling
Logistic Regression model
Hyperparameter tuning using Optuna
Model evaluation using multiple metrics
Model serialization using Joblib

📂 Dataset
The project uses three datasets:
customers.csv
loans.csv
bureau.csv

These datasets are merged using the common customer ID to create the final training dataset.

🛠️ Technologies Used
Python
Pandas
NumPy
Matplotlib
Scikit-learn
Statsmodels
Optuna
Joblib
Jupyter Notebook

📊 Project Workflow
1. Data Loading
Load customer, loan, and bureau datasets
Merge datasets
2. Data Cleaning
Handle missing values
Remove duplicates
Fix inconsistent categorical values
Validate business rules
3. Exploratory Data Analysis (EDA)
Distribution plots
Boxplots
KDE plots
Class imbalance analysis
Target variable analysis
4. Feature Engineering

Created several useful features including:
Loan-to-Income Ratio
Delinquency Ratio
Average DPD per Delinquency
Removed unnecessary ID columns and business-restricted features.

5. Feature Selection
Removed multicollinear features using VIF
Encoded categorical variables
Standardized numerical features
6. Model Building
Implemented:
Logistic Regression
Performed hyperparameter tuning using Optuna.

7. Model Evaluation
The model was evaluated using:
Accuracy
Precision
Recall
F1 Score
ROC Curve
AUC Score
KS Statistic
Gini Coefficient
Rank Ordering (Decile Analysis)
8. Model Saving

The final trained model is saved using Joblib for future predictions.

📈 Evaluation Metrics

The notebook evaluates the model using industry-standard credit risk metrics:

ROC Curve
Area Under Curve (AUC)
KS Statistic
Gini Coefficient
Decile-wise Rank Ordering
Event Rate Analysis

These metrics are commonly used in banking and financial risk modeling.

📁 Project Structure
ML_Project_Credit_Risk_Prediction/
│
├── dataset/
│   ├── customers.csv
│   ├── loans.csv
│   └── bureau.csv
│
├── credit_risk_model.ipynb
├── requirements.txt
├── README.md
└── saved_model.joblib
▶️ How to Run
Clone Repository
git clone https://github.com/your-username/ML_Project_Credit_Risk_Prediction.git
Install Dependencies
pip install -r requirements.txt
Run Jupyter Notebook
jupyter notebook

Open:

credit_risk_model.ipynb
📦 Requirements

Example packages:
pandas
numpy
matplotlib
scikit-learn
statsmodels
optuna
joblib
jupyter

💡 Key Learnings
Data preprocessing for financial datasets
Credit risk modeling
Feature engineering techniques
Handling class imbalance
Model optimization using Optuna
Credit scoring evaluation metrics
Model deployment preparation

🎯 Future Improvements
XGBoost
LightGBM
CatBoost
Random Forest
Explainability using SHAP
Streamlit Web App
MLflow Experiment Tracking
Docker Deployment
CI/CD Pipeline
