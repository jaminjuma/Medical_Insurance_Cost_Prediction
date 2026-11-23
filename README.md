# 🏥 Medical Insurance Cost Prediction — Regression Modeling

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.x-blue?logo=python&logoColor=white" alt="Python">
  <img src="https://img.shields.io/badge/Pandas-Data%20Analysis-150458?logo=pandas&logoColor=white" alt="Pandas">
  <img src="https://img.shields.io/badge/scikit--learn-Modeling-F7931E?logo=scikitlearn&logoColor=white" alt="scikit-learn">
  <img src="https://img.shields.io/badge/Seaborn-Visualization-4C72B0" alt="Seaborn">
  <img src="https://img.shields.io/badge/Status-In%20Progress-orange" alt="Status">
  <img src="https://img.shields.io/badge/License-MIT-yellow" alt="License">
</p>

<p align="center">
  An end-to-end regression project that predicts <b>annual medical insurance cost</b> from patient
  attributes — from raw CSV to a baseline Linear Regression model and honest evaluation.
</p>

---

## 📖 Overview

This project builds a model to predict how much a patient is charged for medical insurance coverage
based on attributes such as age, BMI, smoking status, number of children, and region.
The goal is to answer a practical question with real evidence: **which patient factors drive insurance
cost, and how accurately can we predict it?**

The notebook covers:

- 🎯 **Problem definition** — problem type, target, success criteria, and end users
- 🧹 **Cleaning** — checking types, duplicates, and missing values
- 🔍 **Exploration** — distributions and relationships between features and cost
- 🤖 **Modeling** — Linear Regression baseline with train/test evaluation
- 📈 **Evaluation** — error metrics and checks for overfitting/underfitting

---

## 🎯 Problem Definition

**Problem type:** Regression — the target variable is continuous.
A Linear Regression model is used as the baseline to learn the relationship between patient attributes
and insurance cost.

**Target variable:** `charges` — the annual medical insurance cost billed to a patient.

**What does a good prediction mean?**
A good prediction generalizes well to unseen data, avoiding both overfitting and underfitting. The model
should achieve low error while keeping performance stable across the training and test sets.

**Who would use this prediction?**
- Insurance companies, to set fair and consistent premiums
- Government health insurance programs, to support data-driven policy decisions and reduce bias in
  premium allocation

---

## 🗂️ Dataset

| Detail | Description |
|---|---|
| **Source** | <Kaggle – Medical Cost Personal Dataset / your source> |
| **File** | `insurance.csv` |
| **Size** | <~1,338 rows, 7 columns> |
| **Target** | `charges` |
| **Features** | `age`, `sex`, `bmi`, `children`, `smoker`, `region` |

> 📥 Download the dataset from Kaggle and place it in the working directory before running the notebook.

---

## 🧹 Data Cleaning & Preparation

1. **Inspected structure and data types** (`info()`, `describe()`)
2. **Checked and removed duplicate rows**
3. **Checked for missing values** and handled them where needed
4. **Encoded categorical features** (`sex`, `smoker`, `region`) for modeling
5. **Split the data** into training and test sets (<80/20>, `random_state=<42>`)

---

## 📊 Exploratory Analysis

| Plot | What it shows |
|---|---|
| **Histogram** | Distribution of `charges` and key numeric features |
| **Box plot** | Charges by smoker status, sex, and region |
| **Scatter plot** | Charges vs. age and BMI |
| **Correlation heatmap** | Linear relationships between numeric features and charges |

**Key findings:** <e.g., smoker status and age are the strongest drivers of cost — fill in from your analysis>

---

## 🤖 Modeling

- **Baseline model:** Linear Regression (`sklearn.linear_model.LinearRegression`)
- **Evaluation metrics:** R², MAE, RMSE
- **Generalization check:** compare train vs. test scores to detect overfitting/underfitting

| Metric | Train | Test |
|---|---|---|
| R² | <0.00> | <0.00> |
| MAE | <0.00> | <0.00> |
| RMSE | <0.00> | <0.00> |

---

## 🛠️ Tech Stack

- **Python** — pandas, numpy
- **Modeling** — scikit-learn
- **Visualization** — matplotlib, seaborn
- **Environment** — developed in Google Colab / Jupyter

---

## 🚀 Getting Started

```bash
# Clone the repo
git clone https://github.com/jaminjuma/<repo-name>.git
cd <repo-name>

# Install dependencies
pip install pandas numpy matplotlib seaborn scikit-learn

# Download insurance.csv from Kaggle and place it in the project folder,
# then run the notebook
jupyter notebook
```

---

## 🔮 Possible Next Steps

- Try Ridge/Lasso regularization to improve generalization
- Compare against tree-based models (Random Forest, Gradient Boosting)
- Feature engineering (e.g., BMI categories, smoker × BMI interaction)
- Log-transform the target to handle skewed charges
- Deploy the model as a simple API or web app

---

## 👤 Author

**Jamin Juma**
Founder of [Automateke](https://automateke.app) · CS student, Kirinyaga University

- 🌐 Portfolio: [jaminjuma.tech](https://jaminjuma.tech)
- 💻 GitHub: [@jaminjuma](https://github.com/jaminjuma)
- 🔗 LinkedIn: [jumajamin](https://linkedin.com/in/jumajamin)

---

## 📄 License

This project is licensed under the MIT License — feel free to use and adapt it.
