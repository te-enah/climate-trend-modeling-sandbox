# Module 1: Exploratory Data Analysis & Correlation Mapping

## 1. Strongest Linear Variables
By computing the Pearson correlation coefficient ($r$) for indicators across the 2000–2020 period using `=CORREL()`, several highly distinct relationships emerged:
* **CO₂ Concentration & Sea Level Rise:** Strongest linear lock in the dataset ($r \approx 0.999$).
* **Global Emissions & CO₂ Concentration:** Strong positive linear coupling ($r \approx 0.915$).
* **CO₂ Concentration & Temperature Anomaly:** Strong positive trend ($r \approx 0.891$).
* **Arctic Ice Extent & Global Emissions:** Strong negative linear trend ($r \approx -0.793$).

---

## 2. Visualizing CO₂ vs. Temperature Anomaly
We mapped our baseline regression curve to see how carbon accumulation patterns correspond to rising global anomalies. Roughly **79.4%** of the variance in global temperatures is explained purely by the linear increase in atmospheric CO₂ concentration ($R^2 = 0.794$).

### 🖼️ Regression Baseline Chart
  <img width="1522" height="528" alt="Global Temperature Anomalies vs  Atmospheric CO2 Concentratio" src="https://github.com/user-attachments/assets/2744178f-8bba-4a1c-b7cd-ca9642a6844a" />


**Linear Model Formulation:**
$$\text{Temperature Anomaly} = 0.0146(\text{CO}_2) - 4.96$$
