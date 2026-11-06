# Customer Churn Prediction Using Machine Learning

## Project Overview

This project focuses on predicting whether a telecom customer is likely to leave a company using supervised machine learning algorithms.

The project uses customer demographic, account, service, and billing information to identify potential customer churn. It includes data preprocessing, exploratory data analysis, feature encoding, handling class imbalance, model training, hyperparameter tuning, and performance evaluation.

## Dataset

- **Dataset:** Telco Customer Churn
- **Total Records:** 7,043
- **Target Variable:** `Churn`
- **Problem Type:** Binary Classification

The target variable indicates whether a customer has discontinued the telecom service.

## Project Workflow

1. Data Loading and Exploration
2. Data Cleaning and Preprocessing
3. Missing Value Handling
4. Exploratory Data Analysis (EDA)
5. Feature Selection
6. Categorical Feature Encoding
   - Binary Encoding
   - One-Hot Encoding
7. Train-Test Split
8. Handling Class Imbalance Using SMOTE
9. Random Forest Model Training
10. XGBoost Model Training
11. Hyperparameter Tuning Using GridSearchCV
12. Model Evaluation
13. ROC Curve Comparison
14. Feature Importance Analysis

## Machine Learning Models

### 1. Random Forest Classifier

Random Forest is an ensemble learning algorithm that combines multiple decision trees to make predictions. It is used to classify customers into churn and non-churn categories.

### 2. XGBoost Classifier

XGBoost (Extreme Gradient Boosting) is an ensemble learning algorithm that builds decision trees sequentially to improve prediction performance.

GridSearchCV with 5-fold cross-validation is used for hyperparameter tuning, while SMOTE is integrated into the training pipeline to handle class imbalance.

## Model Evaluation

The models are evaluated using the following performance metrics:

- Accuracy
- Precision
- Recall
- F1-Score
- ROC-AUC Score
- Confusion Matrix
- ROC Curve

### XGBoost Performance

| Evaluation Metric | Score |
|---|---:|
| Accuracy | 77.34% |
| Precision | 56.15% |
| Recall | 76.20% |
| F1-Score | 64.66% |
| ROC-AUC | 84.05% |

### ROC-AUC Comparison

| Model | ROC-AUC |
|---|---:|
| Random Forest | 0.827 |
| XGBoost | 0.840 |

XGBoost achieved a slightly higher ROC-AUC score than Random Forest, indicating better ability to distinguish between churn and non-churn customers on the test dataset.

## Technologies and Libraries

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Imbalanced-learn
- XGBoost
- Jupyter Notebook

## Repository Structure

```text
Customer-Churn-Prediction/
│
├── Customer_Churn_Prediction.ipynb
├── README.md
├── requirements.txt
├── .gitignore
└── WA_Fn-UseC_-Telco-Customer-Churn.csv
```

*The dataset CSV should be included only if its distribution license permits redistribution.*

## How to Run the Project

1. Clone or download this repository.
2. Install the required dependencies using `requirements.txt`.
3. Place the dataset CSV in the project directory.
4. Open the Jupyter Notebook.
5. Run the notebook cells in sequence.

Install dependencies:

```bash
pip install -r requirements.txt
```

## Future Improvements

- Deploy the churn prediction model using Streamlit or Flask.
- Improve feature engineering.
- Experiment with additional machine learning algorithms.
- Optimize model performance through further hyperparameter tuning.
- Apply explainable AI techniques such as SHAP.

## Author

**Zeyan Khan**
