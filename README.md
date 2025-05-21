# -Bank-Churn-Prediction-Using-LightGBM
Predicting customer churn is critical for banks aiming to improve customer retention and reduce revenue loss. This project leverages the power of **LightGBM**, a high-performance gradient boosting framework, to build a classification model that predicts whether a customer is likely to leave the bank.
## 🎯 Project Objective

To build an accurate and interpretable machine learning model that predicts **customer churn** using structured customer demographic and account-related data.

## 📂 Dataset Description

The dataset contains customer-level information from a fictional bank and includes the following features:

- **Customer Profile**: Age, Gender, Geography
- **Account Information**: Credit Score, Balance, Tenure, Number of Products
- **Customer Behavior**: Has Credit Card, Is Active Member
- **Financial Metrics**: Estimated Salary
- **Target Variable**: `Exited` — whether the customer left the bank (1) or not (0)

## 🔍 Exploratory Data Analysis (EDA)

- Visualized class imbalance of churn (only ~20% exited)
- Checked distributions of numeric features (age, balance, salary, etc.)
- Analyzed correlations and feature importance
- Encoded categorical variables using one-hot and label encoding where appropriate
- Identified skewed features and scaled them

## ⚙️ Modeling Approach

- Model used: **LightGBM Classifier**
- Key techniques:
  - **Train-test split** (80/20)
  - **Early stopping** to prevent overfitting
  - **Hyperparameter tuning** using basic grid-based parameters
  - **Class imbalance handling** via parameter adjustment or weighting
- Evaluation metrics:
  - **Accuracy**
  - **Precision, Recall, F1-Score**
  - **Confusion Matrix**
  - **ROC-AUC Score**

## 📊 Results & Insights

| Metric           | Score        |
|------------------|--------------|
| Accuracy         | *e.g., 86.5%* |
| ROC-AUC Score    | *e.g., 91.2%* |
| Precision        | *e.g., 78%*   |
| Recall (Churn)   | *e.g., 71%*   |

- **LightGBM** provided excellent performance with fast training and strong predictive power.
- Most influential features: **Age**, **Balance**, **Number of Products**, and **Is Active Member**.
- The model was able to detect a significant proportion of true churners, which is critical for retention strategies.

## 📦 Tools & Technologies

- **Python**
- **Pandas**, **NumPy** for data processing
- **Matplotlib**, **Seaborn** for visualization
- **LightGBM** for modeling
- **scikit-learn** for preprocessing and evaluation
