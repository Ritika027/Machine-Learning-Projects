# Credit Scoring Model

## Overview
The **Credit Scoring Model** is a Machine Learning project that predicts whether an individual is **creditworthy or not** based on their financial history. Financial institutions use such models to assess the risk of lending money to customers.

This project uses classification algorithms to analyze financial attributes and determine whether a person is eligible for credit.

---

## Objective
The main objective of this project is to build a **machine learning classification model** that predicts an individual's creditworthiness using past financial data.

---

## Features
- Data preprocessing and cleaning
- Feature engineering from financial data
- Implementation of multiple classification models
- Performance evaluation using standard metrics
- Comparison of different algorithms

---

## Machine Learning Algorithms Used
- Logistic Regression
- Decision Tree Classifier
- Random Forest Classifier

---

## Dataset Features

| Feature | Description |
|-------|-------------|
| Income | Annual income of the individual |
| Debts | Total outstanding debt |
| Payment_History | Past payment behavior |
| Credit_Utilization | Percentage of credit used |
| Loan_Amount | Requested loan amount |
| Credit_Score | Historical credit score |

### Target Variable
`Creditworthy`

- **1 → Credit Approved**
- **0 → Credit Denied**

---

## Project Workflow
1. Data Collection
2. Data Preprocessing
3. Feature Engineering
4. Train-Test Split
5. Model Training
6. Model Evaluation

---

## Evaluation Metrics
The models are evaluated using the following metrics:

- **Precision**
- **Recall**
- **F1-Score**
- **ROC-AUC Score**

These metrics help measure the performance and reliability of the credit scoring model.

---

## Technologies Used
- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Seaborn

---

## Installation

Clone the repository:

```bash
git clone https://github.com/your-username/credit-scoring-model.git
```

Install required libraries:

```bash
pip install pandas numpy scikit-learn matplotlib seaborn
```

---

## Running the Project

Run the Python script:

```bash
python credit_scoring_model.py
```

---

## Expected Output
The model generates classification performance metrics including:

- Precision
- Recall
- F1-score
- ROC-AUC score

These results indicate how accurately the model predicts creditworthiness.

---

## Future Improvements
- Hyperparameter tuning
- Adding more financial features
- Using advanced models such as XGBoost
- Deploying the model as a web application

---
