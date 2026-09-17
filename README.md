# 🛒 SmartKart Customer Churn Intelligence

### End-to-End Machine Learning Pipeline for Customer Churn Prediction

SmartKart Customer Churn Intelligence is an end-to-end machine learning project that analyzes customer data, cleans real-world data-quality issues, identifies churn patterns, predicts customers at risk of leaving, and generates a business-ready churn risk report.

The project uses **Logistic Regression** to predict customer churn based on **Age, Monthly Spend, and Complaints**, following a complete 15-step machine learning pipeline.

## 📁 Repository Name

```text
smartkart-customer-churn-intelligence
```

## 📂 Recommended Repository Structure

```text
smartkart-customer-churn-intelligence/
│
├── 📓 SmartKart_Churn_Prediction_ML_Pipeline.ipynb
├── 📊 SmartKart_dirty_100_rows.csv
├── 📄 smartkart_churn_risk_report.csv
└── 📖 README.md
```

## 🎯 Project Goal

The goal is to predict which SmartKart customers are likely to **churn**, allowing a retention team to identify high-risk customers and take action before they leave.

## 🤖 Machine Learning Model

**Logistic Regression**

### Input Features

* `Age`
* `Monthly_Spend`
* `Complaints`

### Target

* `Churn = 0` → No Churn
* `Churn = 1` → Churn

`Customer_ID` is retained for customer identification but excluded from model training.

## 🔄 15-Step Pipeline

```text
Data Collection
      ↓
Data Understanding
      ↓
Data Cleaning
      ↓
Outlier Detection & Treatment
      ↓
Feature Selection
      ↓
Target Definition
      ↓
Target Encoding
      ↓
Train-Test Split
      ↓
Feature Standardisation
      ↓
Model Building
      ↓
Model Training
      ↓
Prediction
      ↓
Model Evaluation
      ↓
Model Interpretation
      ↓
Final Business Output
```

## 📊 Model Performance

| Metric    |   Result |
| --------- | -------: |
| Accuracy  |     ~89% |
| Precision |     ~83% |
| Recall    | **100%** |
| F1-Score  |     ~91% |

The notebook evaluates the model using a confusion matrix, accuracy, precision, recall and F1-score.

> **Note:** The evaluation is based on a relatively small test set, so these results should be treated as educational/portfolio results rather than production-level validation.

## 💡 Key Business Insights

* Higher **Monthly Spend** is associated with lower predicted churn risk.
* Higher **Complaints** are associated with increased churn risk.
* **Age** has the weakest modeled relationship with churn among the three features.

## 🚨 Final Output

The system produces a ranked customer churn-risk report containing:

```text
Customer_ID
Age
Monthly_Spend
Complaints
Actual_Churn
Predicted_Churn
Churn_Probability
Risk_Label
```

Customers are sorted by churn probability so the highest-risk customers can be prioritized for retention action.

## 🛠️ Tech Stack

```text
Python
Pandas
NumPy
Scikit-learn
Matplotlib
Seaborn
Google Colab / Jupyter Notebook
```

## 🚀 Future Scope

* Larger customer datasets
* More behavioural features
* Random Forest / XGBoost comparison
* Hyperparameter tuning
* Cross-validation
* Interactive Streamlit dashboard
* Automated retention recommendations

---

### 👨‍💻 Project

**SmartKart Customer Churn Intelligence**

A practical application of machine learning for **customer retention, predictive analytics, and business intelligence**.
