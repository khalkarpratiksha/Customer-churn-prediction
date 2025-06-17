# 📊 Customer Churn Prediction Project

This project predicts whether a customer is likely to churn (discontinue the service) based on their usage and demographic data using machine learning models. The primary goal is to help telecom companies take proactive steps to retain high-risk customers.

---

## 📌 Problem Statement

Customer churn is a significant problem for subscription-based businesses like telecommunications. This project aims to build a predictive model that can identify customers who are likely to churn. By detecting them early, businesses can take strategic actions (like discounts or personalized offers) to retain them.

---

## 🗃️ Dataset Description

The dataset contains customer details such as:

- `customerID`, `gender`, `SeniorCitizen`, `Partner`, `Dependents`
- `tenure`, `PhoneService`, `MultipleLines`, `InternetService`, `OnlineSecurity`, `OnlineBackup`, `DeviceProtection`, `TechSupport`, `StreamingTV`, `StreamingMovies`
- `Contract`, `PaperlessBilling`, `PaymentMethod`
- `MonthlyCharges`, `TotalCharges`
- **Target**: `Churn` (Yes or No)

🧹 Data Preprocessing:
- Dropped `customerID` column
- Converted `TotalCharges` to numeric
- Encoded categorical columns using one-hot encoding
- Standardized numerical features using `StandardScaler`

---

## 🧠 Models Used

The following machine learning models were trained and evaluated:

- **Logistic Regression**
- **Random Forest Classifier**
- (Optional) **XGBoost Classifier**

---

## 📊 Model Performance

| Model              | Accuracy | Recall (Churn=1) | F1-Score (Churn=1) | Comments |
|--------------------|----------|------------------|--------------------|----------|
| Logistic Regression| 78.75%   | 52%              | 56%                | Performs well on non-churners |
| Random Forest      | 78.46%   | 50%              | 54%                | Slightly lower recall on churners |

📌 **Key Insight**: Recall for churners (class `1`) is more important than overall accuracy because the business needs to correctly identify customers who are about to leave.

---

## 📁 Project Structure

