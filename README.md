# Evaluating Climate Indicator Trendlines: A Regression and Diagnostic Analysis (2000–2020)

## 📌 Project Overview
This project evaluates how effectively simple statistical models can predict global temperature changes, CO₂ levels, and sea-level rise. Using a 21-year dataset of annual global climate indicators, we investigate the mechanics of regression analysis, error metrics, and model optimization directly within spreadsheet environments.

---

## 📂 Project Directory (Modules)

To explore the step-by-step breakdown of this research, navigate through the specific project modules below:

* ### 📊 [Module 1: Exploratory Data Analysis](./modules/01_exploratory_analysis.md)
  Initial statistical pairings, Pearson correlation ($r$) mappings, and evaluating core baseline relationships like CO₂ vs. Temperature Anomalies.
  
* ### 📉 [Module 2: Regression & Residual Diagnostics](./modules/02_residual_diagnostics.md)
  Building the linear trendline model, calculating actual vs. predicted values, and decoding the structural U-shaped diagnostic warning sign.
  
* ### 🧠 [Module 3: Polynomial Optimization & Bias-Variance Tradeoff](./modules/03_model_optimization.md)
  Testing higher-degree polynomial trends (Degrees 2–4), defining macro accuracy metrics (MAE, MSE, RMSE), and navigating the physics of thermal climate lags.

---

## 🛠️ Global Spreadsheet Toolset Used
* **Model Coefficients:** `=SLOPE()`, `=INTERCEPT()`
* **Linear Tracking:** `=CORREL()`
* **Error Engine Matrix:** `=SUMPRODUCT(ABS())`, `=SQRT(SUMPRODUCT())`
