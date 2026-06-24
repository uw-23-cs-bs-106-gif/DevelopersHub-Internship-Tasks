# 🏦 Task 2: Loan Eligibility Prediction & Credit Risk Analysis

This directory contains the professional analytical workspace and machine learning architecture built to address **Task 2: Predictive Classification on Financial Datasets**. 

The task focuses on implementing an end-to-end predictive classification pipeline to determine loan approval viability (`Loan_Status` $\rightarrow$ `Y/N`) using applicant financial metrics, credit histories, and socio-demographic profiles.

---

## 🛠️ Core Analytical Workflow & Architecture
The entire data science workflow is meticulously fully contained inside the `DHC_TASK2.ipynb` Jupyter Notebook, structured as follows:

1. **Robust Exploratory Data Analysis (EDA):** Characterization of the baseline layout containing **614 records across 13 dimensional attributes**. Includes analyzing target skewness (`Y`: 422 vs. `N`: 192).
2. **Missing Value Imputation Strategy:** Systematic handling of missing values using feature-appropriate strategies to prevent data leakage:
   * **Categorical Imputation (Mode):** `Gender` (Male), `Married` (Yes), `Dependents` (0), `Self_Employed` (No), and `Credit_History` (1.0).
   * **Numerical Imputation (Median):** `LoanAmount` (128.0) and `Loan_Amount_Term` (360.0).
3. **Advanced Feature Engineering:** Transformation of structural arrays including skewed feature mitigation via mathematical transformations (log-transformations applied to `ApplicantIncome` and `LoanAmount` to promote model convergence and stability).
4. **Machine Learning Pipeline Evaluator:** Construction and tuning of a predictive model suite headlined by an optimized **Random Forest Classifier** (`max_depth=6`, `n_estimators=100`).

---

## 📋 Features & Data Dimensions

The dataset evaluates loan requests across the following structural dimensions:

* **Demographic Vectors:** `Gender`, `Married`, `Dependents`, `Education`, `Self_Employed`
* **Financial Position Metrics:** `ApplicantIncome`, `CoapplicantIncome`, `LoanAmount`, `Loan_Amount_Term`
* **Risk & Geography Profiles:** `Credit_History` (Primary factor), `Property_Area` (Urban, Semi-Urban, Rural)
* **Target Classification:** `Loan_Status` (Approved `Y` / Rejected `N`)

---

## 🎯 Empirical Insights & Conclusions

From the model outputs and comparative analytics, the following production conclusions were derived:
* **🥇 Strongest Predictor:** `Credit_History` is statistically verified as the most powerful determinant for approval mechanics. A positive history maps directly to a **>80% benchmark approval rate**.
* **📈 Best Architecture:** **Random Forest** exhibits superior out-of-sample generalization capacity, achieving optimal ROC-AUC boundaries.
* **🗺️ Regional Variance:** Applicants seeking properties within **Semi-Urban** geographical pockets demonstrate higher raw approval rates compared to alternative structural segments.
* **⚖️ Ethical Alignment:** Features such as `Gender` and `Self_Employed` indicate statistically negligible predictive weights, verifying the fairness and bias-free behavior of the model.

---
