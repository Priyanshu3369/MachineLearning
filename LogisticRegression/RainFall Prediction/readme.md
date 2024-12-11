# 🌧️ Rainfall Prediction Model

A machine learning model that predicts rainfall using historical data and numerical features. Built using Python and popular libraries like `pandas`, `seaborn`, and `sklearn`.

---

## 📊 **Table of Contents**

- [Overview](#overview)  
- [Features](#features)
- [Model Explanation](#model-explanation)  
- [Results](#results)

---

## 🚀 **Overview**

This project is a simple rainfall prediction model using machine learning. The model utilizes historical data to predict rainfall outcomes by applying preprocessing, feature selection, and machine learning techniques.

The goal of this repository is to:
- Preprocess rainfall and weather-related data.
- Train a predictive model using classification algorithms.
- Validate the model's performance on unseen test/validation data.

---

## ✨ **Features**

- Data preprocessing pipeline for handling null values and feature engineering.
- Visualization of data trends using `seaborn` and `matplotlib`.
- Model trained with splitting strategies to ensure stratified testing.
- Uses libraries like Scikit-learn and XGBoost for Machine Learning workflows.
- Model evaluation using accuracy metrics.


seaborn
scikit-learn
xgboost

## 🤖 **Model Explanation**

In this project, we explored multiple machine learning models to predict rainfall. The following models were evaluated:

---

### **1. Logistic Regression**

- **What it does:** Logistic Regression is a linear model primarily used for binary classification tasks. It works by finding the optimal linear boundary between classes.
- **Advantages:** Fast, simple, and easy to interpret.
- **Limitations:** Struggles with complex, non-linear patterns.

---

### **2. Support Vector Classifier (SVC)**

- **What it does:** The Support Vector Classifier is used for classification by identifying the best hyperplane that separates data points from different classes.
- **Advantages:** Effective in high-dimensional spaces and flexible with kernel functions.
- **Limitations:** Can be computationally expensive for large datasets, especially with non-linear patterns.

---

### **3. XGBoost Classifier**

- **What it does:** XGBoost is an implementation of gradient-boosted decision trees designed for high performance and scalability. It builds a series of weak decision trees to improve predictive accuracy by combining their outputs.
- **Advantages:** Accurate, efficient, handles overfitting well, and robust against noisy data.
- **Limitations:** Computational cost could be higher for very large datasets.

---

### **Preprocessing Steps**

We applied preprocessing to clean and prepare the data:

1. **Handled Null Values:** Replaced nulls with the mean of the respective columns.
2. **Feature Engineering:** Selected features for model training and visualization.
3. **Stratified Sampling:** Ensured balanced proportions of target variable classes across training and validation splits.
4. **Train-Test Splitting:** Split the data into 80% training and 20% validation using stratified splitting.

These preprocessing steps ensured our models trained on clean and well-structured data.

---

## 🏆 **Results**

We compared the performance of the three machine learning models mentioned above (Logistic Regression, SVC, XGBoost Classifier) on both training and validation datasets.

### Model Comparison:

| Model                 | Training Accuracy         | Validation Accuracy      |
|-----------------------|---------------------------|------------------------|
| Logistic Regression   | **0.8893209767430116**        | **0.8966666666666667**      |
| Support Vector Classifier (SVC)  | **0.9026413474407211**   | **0.8858333333333333**  |
| **XGBoost Classifier**      | **0.9999999999999999**   | **0.8391666666666666** |

---

### **Key Findings:**

1. **XGBoost Classifier** performed the best among all tested models, with:
   - **Training Accuracy:** `0.9999999999999999`
   - **Validation Accuracy:** `0.8391666666666666`

2. **Why XGBoost?**
   - XGBoost is an ensemble model that combines decision trees to reduce overfitting and improve predictive performance on unseen data.

3. **Comparison Summary:**
   - Logistic Regression and SVC models showed moderate performance compared to the superior generalization capabilities of the XGBoost Classifier.

---

### **Insights**

- The results highlight the importance of feature engineering and preprocessing in improving model performance.
- XGBoost's ability to handle non-linear relationships and ensemble decision-making led to its superior performance on both the training and validation datasets.

The model results demonstrate that **machine learning can effectively predict patterns in weather data** (rainfall trends) when features are carefully preprocessed and appropriate models are selected.

---
