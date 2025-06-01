# Stroke Risk Exploratory Data Analysis

## Summary

This project presents a comprehensive exploratory data analysis (EDA) on a healthcare dataset focused on stroke risk factors. The goal is to uncover the statistical distributions, potential patterns, and key relationships between patient attributes (demographics, lifestyle, and clinical indicators) and stroke occurrence. This EDA forms the groundwork for future predictive modeling efforts aimed at stroke prediction and prevention.

---

## Problem Description

Stroke remains one of the leading causes of death and disability worldwide. While many strokes are preventable through early detection and intervention, identifying individuals at high risk remains a challenge. Utilizing real-world healthcare data allows us to examine how various factors—such as age, hypertension, diabetes, obesity, heart disease, smoking, and lifestyle choices—correlate with stroke incidence. This analysis contributes to both public health understanding and serves as a strong applied data science exercise.

---

## Motivation

- Apply data science techniques to a real-world healthcare problem.
- Explore risk factors contributing to stroke using statistical and visual analysis.
- Provide a foundation for future machine learning models that can assist in clinical decision support.
- Demonstrate technical expertise in EDA for professional portfolio purposes.

---

## Dataset Description

The dataset used for this project is the **Healthcare Stroke Prediction Dataset** sourced from Kaggle. It contains health information from 5,110 patients.

| Feature | Description |
|---------|-------------|
| id | Unique patient identifier |
| gender | Male, Female, Other |
| age | Patient's age (0.08 to 82 years) |
| hypertension | 0 = No, 1 = Yes |
| heart_disease | 0 = No, 1 = Yes |
| ever_married | Yes / No |
| work_type | Private, Self-employed, Govt_job, children, Never_worked |
| residence_type | Urban / Rural |
| avg_glucose_level | Average blood glucose level (55.12 - 271.74 mg/dL) |
| bmi | Body Mass Index (10.3 - 97.6) |
| smoking_status | formerly smoked, never smoked, smokes, Unknown |
| stroke | 0 = No, 1 = Yes (Target variable, highly imbalanced ~4.87%) |

---

## Methodology

1. **Data Cleaning:** Load data, verify missing values, handle categorical encoding.
2. **Descriptive Statistics:** Summary statistics for numeric & categorical variables.
3. **Visualization:** Histograms, boxplots, countplots, KDEs, bivariate analysis.
4. **Correlation Analysis:** Numerical correlation matrix.
5. **Findings Interpretation:** Key insights & preparation for predictive modeling.

---

## Key Findings

- Stroke strongly associated with **age, hypertension, heart disease, glucose level, BMI**.
- Imbalanced target variable: only ~4.87% stroke cases.
- Bimodal age distribution: infants & middle-aged adults dominate dataset.
- Significant missing data (~30%) in smoking status.
- Categorical imbalances (e.g. 'work_type', 'ever_married', 'gender') addressed during EDA.
- Weak correlations overall between numeric features (max ~0.3).

---

## Future Work

- Build predictive models (classification) for stroke prediction.
- Handle class imbalance (SMOTE, class weights).
- Feature engineering & transformation.
- Model evaluation using F1-score, ROC-AUC.
- Possible deployment as healthcare decision support.

---

## How to Run

1️⃣ Clone this repo  
2️⃣ Install dependencies with:

```bash
pip install -r requirements.txt