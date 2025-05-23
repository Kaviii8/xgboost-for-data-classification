# 📉 Customer Churn Prediction with XGBoost

[![Python](https://img.shields.io/badge/Python-3.8%2B-blue.svg)](https://www.python.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

This project demonstrates how to predict **customer churn** using an XGBoost classifier, with a focus on **data preprocessing**, **model training**, **hyperparameter optimization**, and **evaluation** using the popular **Telco Customer Churn dataset**.

---

## 🚀 Project Overview

The goal is to build a machine learning pipeline that can effectively identify customers who are likely to churn, helping businesses take preemptive actions.

### 🔍 Key Steps in `xgboost_code.ipynb`:

* 📥 **Data Loading** – Load and explore the dataset.
* 🧹 **Data Preprocessing** – Clean and encode categorical features.
* 🧪 **Train-Test Split** – Stratified 80/20 split of the dataset.
* ⚙️ **Model Training** – Build a baseline XGBoost classifier.
* 🔍 **Hyperparameter Tuning** – Optimize model using `GridSearchCV`.
* 📊 **Evaluation** – Assess performance using accuracy, confusion matrix, and balanced metrics.

---

## 🧾 Dataset

* **File**: `WA_Fn-UseC_-Telco-Customer-Churn.csv`
* **Rows/Columns**: 7043 × 21
* **Source**: IBM Sample Data Sets (included in this repo)
* **Description**: Customer demographic data, account info, services subscribed, and churn status.

---

## 📁 File Structure

```bash
├── xgboost_code.ipynb        # Main notebook with full analysis pipeline
├── WA_Fn-UseC_-Telco-Customer-Churn.csv  # Dataset
└── README.md                 # Project description
```

---

## 🛠️ Technologies Used

* **Language**: Python 3.x
* **Libraries**:

  * `pandas`, `numpy` – Data wrangling
  * `scikit-learn` – ML tools & evaluation
  * `xgboost` – Gradient boosting model
  * `matplotlib` – Confusion matrix visualization
  * `jupyterlab` or `notebook` – Development environment

---

## ⚙️ Setup & Installation

1. **Clone the repo**

   ```bash
   git clone https://github.com/Kaviii8/xgboost-for-data-classification.git
   cd customer-churn-xgboost
   ```

2. **Create a virtual environment**

   ```bash
   python -m venv venv
   source venv/bin/activate  # Windows: venv\Scripts\activate
   ```

3. **Install dependencies**
   Create `requirements.txt`:

   ```txt
   pandas
   numpy
   scikit-learn
   xgboost
   matplotlib
   jupyterlab
   ```

   Install:

   ```bash
   pip install -r requirements.txt
   ```

4. **Launch Jupyter**

   ```bash
   jupyter notebook
   ```

---

## 📈 Results Summary

### ✅ Best Parameters from Grid Search:

| Parameter          | Value |
| ------------------ | ----- |
| `max_depth`        | 3     |
| `learning_rate`    | 0.1   |
| `n_estimators`     | 100   |
| `gamma`            | 0.1   |
| `subsample`        | 0.7   |
| `colsample_bytree` | 0.7   |
| `lambda`           | 10    |
| `alpha`            | 1     |

### 🧪 Performance Evaluation:

* `balanced_accuracy_score` used for fair assessment on imbalanced data
* Confusion matrix plotted using `ConfusionMatrixDisplay`
* Results clearly documented in the final notebook cell

---

## 🤝 Contributing

Got suggestions or found a bug? Contributions are welcome!

* 📥 Fork the repository
* 📌 Create a new branch
* ✅ Submit a pull request

---

## 📄 License

This project is licensed under the [MIT License](LICENSE).

---
