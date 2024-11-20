# Bank Marketing Campaign Success Prediction

This project focuses on analyzing and predicting the success of a bank's marketing campaigns, specifically to determine whether customers will subscribe to term deposits. The dataset includes various attributes such as demographic, social, and economic information.

The prediction is performed using three classification models: **Logistic Regression**, **Decision Tree**, and **XGBoost**. The workflow emphasizes feature selection and evaluation metrics to ensure accurate and meaningful predictions.

---

## Dataset Overview

The dataset contains 45,211 entries and 17 columns, including the target variable `y` (whether the customer subscribed to a term deposit). Key attributes include:

- `age`, `job`, `marital status`, `education`
- `balance`, `housing loan`, `contact type`, `campaign details`
- `pdays`, `previous`, `poutcome`
- Target variable `y`: Yes/No (subscribed)

---

## Features

### Data Preprocessing
- **Label Encoding**: Converts categorical data into numerical format.
- **Feature Scaling**: Standardized features using `StandardScaler`.

### Feature Selection
1. **Correlation Analysis**: Selected features with high correlation to the target.
2. **Mutual Information Score**: Ranked features based on their predictive importance.
3. **SelectKBest**: Selected top 10 features using statistical tests.

### Selected Features
`balance`, `previous`, `contact`, `housing`, `age`, `job`, `month`, `duration`, `pdays`, `poutcome`

---

## Models and Evaluation

### Models
1. **Logistic Regression**
2. **Decision Tree**
3. **XGBoost**

### Evaluation Metrics
- Accuracy
- Precision
- Recall
- F1 Score
- Cross-Validation

---

## Instructions to Run

### Prerequisites
- Python 3.8+
- Libraries: `pandas`, `numpy`, `matplotlib`, `seaborn`, `scikit-learn`, `xgboost`

Install the required libraries using:
```bash
pip install -r requirements.txt
