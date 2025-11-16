# 📊 Customer Churn Prediction — Machine Learning Project

This project focuses on understanding customer churn for a DTH/E-Commerce service provider and building predictive models to identify customers who are likely to leave. By analyzing customer behavior, service usage patterns, revenue metrics, complaints, and demographic factors, the project provides a data-driven framework for churn reduction strategies.

---

## 🚀 Project Overview

Customer churn is a major challenge for subscription-based industries. Retaining customers is significantly cheaper than acquiring new ones — making churn prediction a critical business need.

Using a dataset of **11,260 customer accounts** and **19 attributes**, this project performs:

- Exploratory Data Analysis (EDA)
- Data cleaning & feature engineering
- Handling of imbalanced data using **SMOTE**
- Model building using multiple ML algorithms
- Feature importance analysis
- Business recommendations based on insights

---

## 📂 Dataset Summary

- **Total Records:** 11,260  
- **Target Variable:** `Churn` (1 = churned, 0 = not churned)  
- **Features Include:**  
  - Tenure  
  - City tier  
  - Revenue per month  
  - Payment mode  
  - Complaint history  
  - Account segment  
  - Customer service interactions  
  - Cashback, coupon usage  
  - Login device preference  

---

## 🔍 Exploratory Data Analysis (EDA)

Key steps included:

- Treatment of special characters and incorrect data types  
- Handling missing values (median/mode imputation)  
- Outlier detection  
- Univariate, bivariate & multivariate analysis  
- Pairplots & correlation heatmaps  
- Identification of top churn drivers  

**Important observations:**

- Low-tenure customers churn the most  
- Customers with past complaints have higher churn probability  
- “Regular Plus” accounts show maximum churn  
- “Super” accounts show highest retention  
- Churn dataset is highly imbalanced (84%:16%)  

---

## ⚙️ Models Used

Four classification algorithms were evaluated:

1. **Random Forest Classifier**
2. **Logistic Regression**
3. **AdaBoost Classifier**
4. **XGBoost Classifier** (🏆 Best Model)

---

## 🏆 Best Performing Model: XGBoost

XGBoost delivered the highest performance across accuracy, recall, and precision.

**Why XGBoost performed best:**

- Handles non-linear relationships  
- Robust to imbalanced datasets (with proper tuning)  
- Strong feature importance insights  
- High predictive power  

**Top Predictive Features:**

- `Tenure`  
- `Complain_l12m`  
- `Days_since_CC_connect`  
- `Account_segment`  

---

## 📈 Model Evaluation

| Model | Notes |
|-------|-------|
| Random Forest | Good recall but biased towards non-churn class |
| Logistic Regression | Lower accuracy; weaker feature separation |
| AdaBoost | Weak performance on imbalanced data |
| **XGBoost** | **Highest accuracy and best overall performance** |

---

## 🧠 Business Insights

Based on modeling and data analysis:

- Offer **long-tenure plans** to reduce churn among new customers  
- Strengthen **customer service responsiveness** — complaints strongly correlate with churn  
- Promote **Super-tier plans** given their stronger retention  
- Targeted retention offers for **Regular Plus** accounts  
- Run periodic surveys for marital status correlations with churn behavior  

---

## 📌 Files in This Repository

- `notebooks/` — Jupyter notebooks (EDA, cleaning, model training)
- `data/` — (If allowed) processed datasets  
- `models/` — Trained model files (optional)
- `reports/` — PDF report, presentation, visual summaries  
- `README.md` — Project documentation  

---

## 🛠️ Tech Stack

- **Python**
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn
- XGBoost
- Imbalanced-learn (SMOTE)



## ⭐ If you find this useful, please give the repository a star!

