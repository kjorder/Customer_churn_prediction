
# 📉 Customer Churn Prediction

This machine learning project predicts whether a bank customer will churn (i.e., leave the bank) based on their personal and transactional data. The dataset contains 15,000 customer records with various demographic and banking features.

## 📂 Dataset Overview

Each row represents a customer and contains the following features:

- **RowNumber, CustomerId, Surname** – Identifiers
- **Geography** – Country of the customer (e.g., France, Germany, Spain)
- **Gender** – Male/Female
- **Age** – Customer's age
- **CreditScore** – Credit score
- **EstimatedSalary** – Annual income estimate
- **Tenure** – Years the customer has been with the bank
- **NumOfProducts** – Number of products the customer uses
- **HasCrCard** – Whether the customer has a credit card
- **IsActiveMember** – Whether the customer is active
- **Balance** – Bank balance
- **Exited** – Target variable: 1 if the customer left the bank, 0 otherwise

## 🔍 Objective

The goal is to predict the **Exited** value (churn) using classification algorithms.

## 🧠 Models Used & Performance

| Model               | Accuracy | ROC AUC |
|--------------------|----------|---------|
| Random Forest       | 0.89     | 0.80    |
| Logistic Regression | 0.87     | 0.75    |
| XGBoost             | 0.88     | 0.80    |
| SVC                 | 0.88     | 0.74    |
| Decision Tree       | 0.83     | 0.79    |

> The **Random Forest** and **XGBoost** models performed best in both accuracy and ROC AUC.

## 📊 Evaluation Metrics

- Accuracy
- ROC AUC Score
- Precision / Recall
- F1 Score
- Confusion Matrix

## 📈 Visualizations

- Feature distribution plots
- Correlation heatmap
- Churn vs non-churn comparison
- Feature importance from Random Forest
- ROC Curve (see below)

## 🧠 Tech Stack

- Python
- Pandas, NumPy
- Scikit-learn
- XGBoost
- Matplotlib, Seaborn

## 📈 ROC Curves

Below is the ROC curve comparison for all models:

![ROC Curve](images/roc_curve.png)

## 🗂 Project Structure

```
customer-churn-prediction/
├── churn_notebook.ipynb        # Full workflow: EDA, modeling, evaluation
├── requirements.txt            # Dependencies
├── README.md                   # Project overview
└── data/
    └── churn.csv               # Dataset (not shared if private)
```

## 🚀 How to Run

1. Clone the repository or download the ZIP:
```bash
git clone https://github.com/kjorder/customer-churn-prediction.git
```

2. Open `churn_notebook.ipynb` in [Google Colab](https://colab.research.google.com/) or Jupyter Notebook.

3. Install required libraries:
```bash
pip install -r requirements.txt
```

4. Run each cell step-by-step.

---

## 📌 Notes

- All identifiers (CustomerId, Surname) were dropped for modeling.
- Label Encoding and One-Hot Encoding used for categorical variables.
- Feature scaling applied to numerical columns.

---

## 📬 Contact

Created by **Kamol aka** – Junior Data Scientist  
📧 Email: kamol.ds@gmail.com  
🔗 GitHub: [kjorder](https://github.com/kjorder)
