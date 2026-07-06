# Module 2: Regression Execution & Residual Diagnostics

## 1. Building the Prediction Engine
Using the native `=SLOPE()` and `=INTERCEPT()` calculations for **Year ($x$) vs. CO₂ Concentration ($y$)**, we established the exact line of best fit formula:
$$\text{Predicted CO}_2 = 2.2048(\text{Year}) - 4041.11$$

In the spreadsheet, a column for `Predicted_CO2` was populated using:
`=2.2048 * A2 - 4041.11`

The `Residual` column was generated using the error delta formula:
`=Actual - Predicted` (or `=B2 - G2`)

---

## 2. The U-Shaped Diagnostic Trap
Plotting the Year against the Residual column produced a stark, systemic **U-shaped pattern** rather than a completely randomized cloud of points.

### 🖼️ Residual Verification Plot
  <img width="1658" height="516" alt="Year vs Residual (ppm)" src="https://github.com/user-attachments/assets/9f091ec0-e898-4162-96c7-3e38c9df6d48" />


### Analytical Takeaway
A high $R^2$ value (which is 0.9968 here) can be a deceptive metric. The clear structural curve in the residuals mathematically proves that the linear model is suffering from **high bias (underfitting)**—it systematically underpredicts values at the boundaries (2000s and 2020) and overpredicts values in the middle.
