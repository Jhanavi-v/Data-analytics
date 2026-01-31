# Diabetes Prediction & Screening Analysis

This repository contains a comprehensive data science pipeline for diabetes risk assessment. The project integrates traditional machine learning with clinical statistical validation to create a reliable screening tool based on both invasive (lab-based) and non-invasive (lifestyle) factors.

## 🔍 Project Overview
The objective of this analysis is to identify key predictors of diabetes and develop a real-time risk calculator. A significant focus was placed on **Exploratory Data Analysis (EDA)** to understand the impact of factors like BMI, Age, and Smoking History on disease prevalence.

## 🚀 Key Pipeline Stages

### 1. Statistical Exploratory Data Analysis (EDA)
Unlike basic analysis, this project uses rigorous statistical testing to validate findings:
* **Continuous Variables:** Used **Welch’s t-tests** and **Cohen’s d** to quantify the effect size of Age, BMI, and Glucose levels.
* **Categorical Variables:** Implemented **Chi-square contingency tests** and **Cramer’s V** to determine the strength of association for lifestyle factors.
* **Visualizations:** Generated class distribution plots, correlation heatmaps, and boxplots for clinical features.

### 2. Multi-Tiered Modeling Strategy
I developed two distinct modeling approaches:
* **Diagnostic Model (All Features):** Utilizes clinical lab values (HbA1c, Blood Glucose) to achieve maximum predictive accuracy.
* **Screening Model (Non-Invasive):** Excludes lab results to simulate a screening environment where only lifestyle factors (Age, BMI, Hypertension) are available.
* **Architectures:** Benchmarked **Logistic Regression** and **Random Forest** (300 estimators) with `balanced_subsample` weighting to address data imbalance.

### 3. Real-Time Risk Calculator
The project concludes with a functional **Diabetes Risk Screening Tool**. This algorithm uses optimized coefficients to convert user inputs (BMI, Age, etc.) into a probability percentage and provides immediate clinical recommendations (High/Moderate/Low risk).

## 🛠️ Tech Stack
* **Language:** Python 3.x
* **Libraries:** * `Scikit-learn`: Pipelines, Random Forest, Logistic Regression, Calibration Curves
    * `Statsmodels`: Logit model and Odds Ratio calculation
    * `SciPy`: T-tests, Chi-square contingency
    * `Pandas` & `NumPy`: Data manipulation
    * `Matplotlib` & `Seaborn`: Advanced visualizations

## 📂 Project Structure
* `DA_Diabetes_finalreport.ipynb`: The primary reproducible notebook containing all cleaning, EDA, and modeling code.
* `figures/`: High-resolution exports of ROC curves, PR curves, and correlation heatmaps.

## 📊 How to Use
1. Clone the repository:
   ```bash
   git clone [https://github.com/Jhanavi-v/Data-analytics.git](https://github.com/Jhanavi-v/Data-analytics.git)
