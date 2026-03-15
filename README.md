# 📊 Portuguese Bank Marketing Analysis

## 📌 Project Overview
This project analyzes the **Portuguese Bank Marketing dataset** to predict whether a customer will subscribe to a **term deposit product** based on demographic, financial, and marketing campaign data.

The objective is to help the bank improve **marketing efficiency** by identifying customers who are more likely to subscribe, reducing unnecessary calls and improving campaign success rates.

---

## 📂 Dataset Information

The dataset contains information from **direct marketing campaigns (phone calls)** conducted by a Portuguese bank.

Each row represents a **customer interaction during a campaign**.

### Target Variable
**y**

- `yes` → Customer subscribed to the term deposit  
- `no` → Customer did not subscribe  

---

## 📦 What This Project Includes

- Data cleaning and preprocessing
- Exploratory Data Analysis (EDA)
- Feature encoding and transformation
- Machine Learning model building
- Model evaluation using classification metrics
- Business insights and marketing recommendations

---

## ⚙️ Model Used

**Logistic Regression**

Logistic Regression was selected because:

- It performs well for **binary classification problems**
- It provides **interpretable probabilities**
- It achieved better **recall for subscribed customers**

---

## 📈 Model Performance

**Accuracy:** `0.8186`

### Classification Report

| Class | Precision | Recall | F1-score | Support |
|------|-----------|--------|---------|--------|
| Not Subscribed (0) | 0.95 | 0.84 | 0.89 | 7265 |
| Subscribed (1) | 0.35 | 0.63 | 0.45 | 971 |

### Confusion Matrix

| Actual \ Predicted | 0 | 1 |
|---|---|---|
| 0 | 6127 | 1138 |
| 1 | 356 | 615 |

---

## 🎯 Key Evaluation Insight

In marketing prediction problems, **Recall is more important than Precision**.

A **False Negative** means the model predicts a customer will not subscribe, but the customer would actually subscribe.

This results in **missed business opportunities**, which is why recall is prioritized.

However, **precision also matters**, because calling too many uninterested customers increases **marketing costs**.

---

## 💡 Business Recommendations

Based on the analysis and model results:

- Target customers with **high predicted subscription probability**
- Avoid contacting customers unlikely to subscribe to **reduce marketing costs**
- Contact customers at the **right time** to increase response rates
- Offer **personalized deposit plans** based on customer profiles
  
## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

---

## 📊 Project Impact

This project demonstrates how **machine learning can support marketing decision-making** by identifying potential customers more effectively.

Using predictive analytics, banks can:

- Improve **campaign conversion rates**
- Reduce **marketing costs**
- Target customers more efficiently
- Make **data-driven marketing decisions**

---
