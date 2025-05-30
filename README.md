# 🏦 Prediction Model for Insolvent Companies

This project aims to develop a machine learning model that predicts whether a company is likely to become insolvent, based on historical financial data.  
The goal is to support risk management decisions by identifying potential bankruptcies in advance.

---

## 📊 Dataset

- **Source**: Publicly available financial data from KOSPI/KOSDAQ companies (2011–2019)
- **Scope**: Excludes financial companies, SPACs, and limited partnerships
- **Features**: 35 financial variables + 9 derived features
- **Target**: Binary classification (Insolvent or not based on debt ratio & interest coverage)

---

## 🧪 Project Workflow

1. **EDA & Labeling**  
   → Outlier detection, visualization, target variable engineering  
2. **Feature Scaling & Selection**  
   → StandardScaler, VarianceThreshold, correlation filtering  
3. **Modeling & Evaluation**  
   → Trained 7 models (Logistic Regression, LightGBM, etc.)  
   → Selected LightGBM with best F1-score of **0.87**  
   → Tuned parameters and prevented data leakage

---

## 🗂️ Notebooks

| File | Description |
|------|-------------|
| `1. EDA.ipynb` | Exploratory data analysis and preprocessing |
| `2. scaling_feature_selection.ipynb` | Feature engineering and selection |
| `3. Data Leakage - Modeling_parameter tuning.ipynb` | Modeling, validation, and performance comparison |

---

## 🔍 Key Insights

- Feature selection significantly improved model generalizability  
- Identified the importance of certain solvency indicators like Debt Ratio and Interest Coverage  
- Careful validation was required to prevent data leakage due to time-series nature

---

## 📁 Project Summary

- Language: Python  
- Libraries: pandas, sklearn, LightGBM, matplotlib  
- Status: Completed  
- Last updated: 2025.04

---

