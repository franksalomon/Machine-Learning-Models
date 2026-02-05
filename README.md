# Customer Satisfaction Prediction — Banking Dataset

Predicting customer satisfaction (scale 1–4) using supervised machine learning models.  
This project was developed during my Master's degree in Mathematical Modeling, Statistics and Computing and focuses on applied data science in a real-world banking scenario.

---

## 🔗 Quick Access

📓 Main Notebook:  
https://github.com/franksalomon/Machine-Learning-Models/blob/main/notebooks/index.ipynb  

📄 PDF Report:  
report/MD_satisfaccion_bancaria_entregable.pdf  

---

## Problem Statement

The goal is to understand how demographic and product-related variables (e.g., education level, income, gender, product ownership) influence customer satisfaction and to build predictive classification models that could support customer retention and service improvement strategies.

---

## Dataset

- Features: education level, income, gender, product ownership, among others  
- Target variable: satisfaction level (1–4)  
- Data anonymized for academic purposes  

---

## Pipeline

- Data loading and cleaning  
- Exploratory Data Analysis (EDA)  
- Feature engineering  
- Model training  
- Model evaluation and comparison  

---

## Models

- Decision Tree  
- Random Forest  
- Neural Network (MLP + SMOTE)  

---

## Evaluation Metrics

- Accuracy  
- Precision / Recall / F1-score  
- Confusion Matrix  
- Cohen’s Kappa  
- ROC-AUC  

---

## Key Results

| Model | Accuracy | F1-score | Kappa | ROC-AUC |
|------|---------|---------|--------|--------|
| Pruned Decision Tree | 0.50 | 0.46 | 0.18 | — |
| Balanced RF + Feature Filter | 0.46 | 0.41 | 0.09 | — |
| Neural Network (MLP + SMOTE) | 0.43 | 0.44 | 0.17 | 0.64 |

---

## Insights

- Age, income and education were consistently among the most influential variables.
- Class imbalance strongly affected intermediate satisfaction levels.
- Neural networks with SMOTE improved detection of minority classes.
- Interpretability vs performance presents a clear trade-off between models.

---

## How to Run

1. Clone the repository  
2. Install dependencies (`scikit-learn`, `imbalanced-learn`, `pandas`, `seaborn`)  
3. Run the main notebook located in `/notebooks/index.ipynb`

---

## Future Work

- Gradient boosting models (XGBoost / LightGBM)
- Ordinal classification approaches
- Probability calibration
- Feature importance with SHAP
