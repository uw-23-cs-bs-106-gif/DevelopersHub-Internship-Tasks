
# 🏦 Task 3: Customer Churn Prediction & Retention Analytics

This directory contains the production-grade predictive classification engine and diagnostic workflow built to address **Task 3: Modeling Customer Attrition and Risk Profiles**.

The objective of this task is to process historical customer behavior parameters to build an end-to-end classification system capable of mapping and predicting customer churn rates, identifying weak operational risk areas, and determining critical retention factors.

---

## 🛠️ Pipeline Architecture & Analytical Workflow
The entire technical deployment is fully documented and structured inside the `DHC_TASK3.ipynb` Jupyter Notebook through the following core operational layers:

1. **High-Volume Data Processing:** Evaluation of an internal benchmark database spanning **10,000 distinct customer profiles across 14 multidimensional features**.
2. **Exploratory Risk Mapping (EDA):** In-depth structural visualization mapping out core behavioral indicators against customer exit vectors (`Exited` $\rightarrow$ `0` for Retained, `1` for Churned).
3. **Robust Feature Sanitization:** Automated preprocessing pipeline handling unnecessary structural tracking records (such as `RowNumber`, `CustomerId`, and `Surname`) and establishing encoded channels for categorical metadata.
4. **Multi-Model Competitive Framework:** Simultaneous training and evaluation optimization across multiple competitive structural baseline classification frameworks. 
5. **Production Matrix Diagnostics:** Rigorous performance scoring leveraging robust mathematical markers such as test Area Under the ROC Curve (**ROC-AUC Score**) and optimal class stability measures (**F1-Score**) to evaluate final classification boundaries.

---

## 📋 Features & Customer Dimensions

The database captures customer behavior profiles across several primary feature segments:

* **Demographic Vectors:** `Geography` (Regional footprints), `Gender`, `Age`
* **Account Portfolio Metrics:** `Tenure` (Account lifespan), `Balance` (Total capital holding), `NumOfProducts` (Active active-product matrix density)
* **Behavior & Credit Indicators:** `CreditScore`, `HasCrCard` (Active credit lines), `IsActiveMember` (Platform activity status), `EstimatedSalary`
* **Target Classification Objective:** `Exited` (Boolean condition checking if the customer churned)
