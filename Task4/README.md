# 🏥 Task 4: Medical Insurance Cost Prediction

This directory contains the analytical workflow and predictive regression architecture built to address **Task 4: Predictive Modeling and Cost Analysis on Medical Datasets**.

The objective of this task is to process historical patient health profiles and demographic vectors to build a robust statistical model using **Linear Regression** capable of predicting future medical charges (`charges`), mapping primary cost factors, and isolating risk characteristics.

---

## 🛠️ Pipeline Architecture & Analytical Workflow
The entire machine learning pipeline is fully structured and executed inside the `DHC_TASK4.ipynb` Jupyter Notebook through the following core operational layers:

1. **Patient Data Characterization:** Evaluation of a historical benchmark database spanning **1,338 unique patient profiles across 7 primary dimensional attributes**.
2. **Exploratory Feature Analysis (EDA):** In-depth visualization mapping core numerical spreads and categorical distributions against final billing costs.
3. **Feature Preprocessing & Encoding:** Automated data cleaning routines that transform categorical attributes (such as `sex`, `smoker`, and `region`) into model-ready numerical formats, alongside feature scaling.
4. **Linear Regression Optimization:** Construction and training of a supervised regression framework to establish numerical beta-coefficients for cost-weight analysis.
5. **Model Evaluation Metrics:** Performance logging using predictive validation checks ($R^2$ Score, Mean Absolute Error, etc.) to assess baseline stability and prediction errors.

---

## 📋 Features & Patient Dimensions

The dataset evaluates insurance requirements across the following structural dimensions:

* **Demographic Vectors:** `age`, `sex` (Male / Female), `children` (Number of dependents)
* **Biometric & Regional Profiles:** `bmi` (Body Mass Index), `region` (Geographic quadrants: Southwest, Southeast, Northwest, Northeast)
* **Primary Health Risk Factor:** `smoker` (Smoking status: Yes / No)
* **Continuous Target Objective:** `charges` (Individual medical insurance costs)

---

## 🎯 Business Insights & Key Conclusions

From the model outputs and directional metrics, the following operational conclusions were derived:
* **🚬 Strongest Cost Driver:** Smoking behavior is statistically verified as the single most powerful weight influencing insurance charges. Smokers consistently incur drastically higher medical bills compared to non-smokers.
* **📊 Biometric Trajectory:** Increasing `bmi` generally correlates with higher continuous medical costs, amplifying significantly when combined with a positive smoking vector.
* **📈 Demographic Scaling:** Patient `age` demonstrates a steady, positive linear impact on insurance charges over time.
* **⚙️ Operational Viability:** The trained **Linear Regression** model successfully maps historical variables to predict costs accurately, allowing insurance underwriters to proactively estimate future claim amounts and identify high-risk segments based on patient lifestyles.
