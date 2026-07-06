# Module 3: Polynomial Optimization & Bias-Variance Tradeoff

## 1. Polynomial Model Performance Summary
To correct the linear model's underfitting, we fitted higher-degree polynomial trend lines to the data.

| Degree | Model Type | Trendline Equation | $R^2$ Value | MAE | MSE | RMSE |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| **1** | Linear | $y = 2.2048x - 4041.11$ | 0.9968 | 0.6490 | 0.5664 | 0.7526 |
| **2** | Quadratic | $y = 0.0202x^2 - 78.8248x + 77392.90$ | **0.9993** | **0.4363** | **0.3104** | **0.3639** |
| **3** | Cubic | $y = 0.0014x^3 - 8.1824x^2 + 16408.15x - 10968757.09$ | 0.9996 | 0.3214 | 0.2010 | 0.2784 |
| **4** | Quartic | $y = -0.0001x^4 + 0.8091x^3 - 2443.53x^2 + 3279748.73x - 1650778413.29$ | 0.9996 | 0.3011 | 0.1890 | 0.2635 |

---

## 2. Navigating the Bias-Variance Tradeoff
* **Why Degree 4 is Overfitting:** While moving from Degree 2 to Degree 4 bumps the $R^2$ slightly up to 0.9996, it introduces **high variance**. The model begins adapting to minor, short-term data fluctuations rather than capturing the core underlying long-term signal, leading to wild boundary trends.
* **The Quadratic Sweet Spot:** The **Degree 2 (Quadratic) model** cuts the RMSE nearly in half (`0.7526 ppm` to `0.3639 ppm`), resolving the structural curve of our residual plot while preserving baseline simplicity.

---

## 3. Climate Indicator Contrast: Sea Level Rise
Repeating this methodology on **Sea Level Rise** revealed distinct physical behavior. Over a short 20-year window, Sea Level Rise acts highly linear ($R^2 = 0.9905$). 

This is an artifact of **Oceanic Thermal Inertia**. Because water has a high specific heat capacity, the global oceans serve as a planetary buffer, smoothing out jagged annual industrial or economic emission spikes into a steady, persistent upward trend.
