# Telco Customer Churn Prediction 📊 Predictive Modeling with XGBoost & Keras MLP

## 📌 Project Overview
This project presents a comparative analysis between two machine learning approaches for predicting customer churn in a telecommunications dataset:
1. **XGBoost Classifier** (Gradient Boosting Ensemble)
2. **Keras Multi-Layer Perceptron (MLP)** (Deep Neural Network)

Customer churn is a critical business metric. Identifying potential churners in advance allows companies to execute proactive retention strategies[cite: 2].

* **Author:** Haritha Kalhara

---

## 📁 Dataset Summary
* **Source:** Telco Customer Churn Dataset
* **Total Records:** 7,043 customers
* **Features:** 20 predictor variables (Demographic, Service usage, Contract/Financial parameters) + 1 Target Variable (`Churn`)
* **Target Variable:** Binary Classification (`Yes` / `No`)

---

## 🛠️ Technologies & Libraries Used
* **Programming Language:** Python 3.x
* **Data Processing & EDA:** Pandas, NumPy, Matplotlib, Seaborn
* **Machine Learning:** Scikit-Learn, XGBoost Classifier
* **Deep Learning:** TensorFlow / Keras (Sequential API, Dense, Dropout, Batch Normalization)
* **Hyperparameter Tuning:** GridSearchCV, Keras Tuner (RandomSearch)

---

## ⚙️ Data Preprocessing Methodology
1. **Missing Value Imputation:** Handled blank values in numerical features like `TotalCharges'.
2. **Categorical Encoding:** Applied One-Hot Encoding for categorical feature transformation
3. **Feature Scaling:** Applied `StandardScaler` to normalize distributions for optimal neural network convergence
4. **Train/Test Split:** Stratified dataset split to maintain target variable ratios

---

## 📊 Model Performance & Results

Both models were evaluated on the unseen test dataset across standard performance metrics[cite: 2]:

| Model | Accuracy | Precision | Recall | F1-Score | ROC-AUC |
| :--- | :---: | :---: | :---: | :---: | :---: |
| **XGBoost Classifier** | **0.8020** | 0.6589 | **0.5267** | **0.5854** | **0.8459** |
| **Keras MLP** | 0.7970 | **0.6705** | 0.4626 | 0.5475 | 0.8411 |

### 🔑 Key Findings & Conclusion
* **Best Model:** **XGBoost Classifier** achieved superior overall performance with a higher **ROC-AUC (0.8459)**, **Recall (0.5267)**, and **F1-Score (0.5854)** compared to Keras MLP[cite: 2].
* **Business Impact:** High Recall is critical in churn prediction to ensure actual churners are identified so retention offers can be served before they leave[cite: 2].

---

## 🚀 How to Run the Project

### Prerequisites
Make sure you have Python 3.8+ installed on your system.

### Step 1: Clone the Repository
```bash
git clone (https://github.com/harithakalhara/churn-prediction-project.git)

