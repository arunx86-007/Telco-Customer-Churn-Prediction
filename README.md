# 📞 Telco Customer Churn Prediction using Machine Learning

## 📖 Overview

This project predicts whether a telecom customer is likely to churn based on customer demographics, account information, and subscribed services. It follows a complete end-to-end machine learning workflow, including data preprocessing, exploratory data analysis, handling imbalanced data, model building, hyperparameter tuning, and deployment using **Streamlit Community Cloud**.

---

## 🎯 Problem Statement

Customer churn is a major challenge for telecom companies. The objective of this project is to build a machine learning model that accurately predicts customer churn, enabling businesses to identify at-risk customers and improve retention strategies.

---

## 📊 Dataset

The dataset contains customer demographic information, account details, subscribed services, billing information, and churn status.

### Target Variable

- **Churn**
  - 0 → Customer Stayed
  - 1 → Customer Churned

### Features

- Customer Demographics
- Senior Citizen
- Partner & Dependents
- Tenure
- Phone Service
- Internet Service
- Online Security
- Device Protection
- Streaming Services
- Contract Type
- Payment Method
- Monthly Charges
- Total Charges
- Other Customer Attributes

---

## 🛠 Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- XGBoost
- Imbalanced-learn
- Joblib
- Streamlit
- Streamlit Community Cloud

---

## ⚙️ Workflow

- Data Cleaning
- Exploratory Data Analysis (EDA)
- Feature Engineering
- Data Preprocessing
- Stratified Train-Test Split
- Handling Imbalanced Data
- Model Building
- Hyperparameter Tuning
- Model Evaluation
- Streamlit Web Application
- Deployment on Streamlit Community Cloud

---

## 🔍 Data Preprocessing

- Missing value handling
- One-Hot Encoding
- Feature Scaling
- Pipeline & ColumnTransformer implementation
- Stratified Train-Test Split
- Imbalanced data handling using:
  - Class Weights
  - SMOTE
  - SMOTETomek

---

## 🤖 Models Evaluated

- Logistic Regression
- XGBoost Classifier

---

## 📈 Logistic Regression Comparison

| Method | Accuracy | Precision | Recall | F1 Score |
|--------|---------:|----------:|--------:|---------:|
| Class Weight | **0.7516** | **0.5201** | **0.7984** | **0.6299** |
| SMOTE | 0.7488 | 0.5173 | 0.7634 | 0.6167 |
| SMOTETomek | 0.7445 | 0.5117 | 0.7634 | 0.6127 |

---

## 🚀 Hyperparameter Tuning

The XGBoost classifier was optimized using **RandomizedSearchCV** with **5-Fold Cross Validation**.

---

## 🏆 Final Model

**Algorithm:** XGBoost Classifier

| Metric | Value |
|---------|------:|
| Accuracy | **0.755** |
| Precision | **0.525** |
| Recall | **0.793** |
| F1-Score | **0.632** |
| ROC-AUC | **0.842** |

The tuned **XGBoost Classifier** achieved the best balance between **Recall**, **F1-Score**, and **ROC-AUC**, making it the final model for deployment.

---

## 💻 Streamlit Application

An interactive web application was developed using **Streamlit**, allowing users to enter customer information and instantly predict whether the customer is likely to churn.

---

## 🌐 Live Demo

The application is deployed on **Streamlit Community Cloud**.

**Live Demo**

https://telco-customer-churn-prediction-4k3aflhwyh5qqn8cekihcy.streamlit.app/

---

## 📂 Project Structure

```text
Telco-Customer-Churn-Prediction/
│
├── app/
│   └── app.py
├── data/
│   └── Telco-Customer-Churn.csv
├── models/
│   └── churn_model.pkl
├── notebook/
├── requirements.txt
└── README.md
```

---

## 🚀 Installation

```bash
git clone https://github.com/your-username/Telco-Customer-Churn-Prediction.git
cd Telco-Customer-Churn-Prediction
pip install -r requirements.txt
streamlit run app/app.py
```

---

## 📌 Dataset

The dataset is already included in the **`data/`** directory. No additional download is required.

---

## 👨‍💻 Author

**Arun Singh**
