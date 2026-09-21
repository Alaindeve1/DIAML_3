# DIAML Assignment 3: Applied Statistical Analysis and Financial Time Series

**Author:** Ndizeye Alain  
**Program:** Master of Science in Information Technology (MSIT)  
**Institution:** Carnegie Mellon University Africa  
**Course:** Data and Information / Machine Learning (DIAML)  

---

## Overview

This repository contains the complete analytical workflow and computational implementation for **Assignment 3**. The project explores hypothesis testing, normality diagnostics, bivariate macro-demographic correlations, and multi-decade financial time series analysis using empirical datasets.

---

## Assignment Structure

### Question 1: Speed of Light (Michelson's 1879 Experiment)
* **Objective:** Investigate whether Albert Michelson's 1879 experimental determinations deviate from the true velocity of light in air ($299,734.5\text{ km/s}$).
* **Methodology:** One-sample Student's $t$-test (two-tailed), Shapiro-Wilk normality testing, systematic bias calculation, and sample size power scaling ($n=200$).
* **Data Source:** `michelson_speed_of_light.json` (Experiment 1, $n=20$).

### Question 2: Chick Weights by Feed Type (Snedecor, 1948)
* **Objective:** Evaluate agricultural weight differences in 6-week-old chicks fed Casein vs. Soybean diets.
* **Methodology:** Independent two-sample Welch's $t$-test (heteroscedastic), Cohen's $d$ effect size, agricultural practical evaluation, and diagnostic boxplot visualization.
* **Data Source:** `chickwts_casein_soybean.csv` ($n=26$).

### Question 3: Fertility Rate vs. GDP per Capita (World Bank 2024)
* **Objective:** Examine the global cross-sectional relationship between Total Fertility Rate and GDP per capita (PPP).
* **Methodology:** Logarithmic vs. linear scaling, tripartite correlation analysis (Pearson raw, Pearson log, Spearman rank), outlier detection ($|z| > 2.5$), and panel/longitudinal econometrics evaluation.
* **Data Source:** World Bank Development Indicators (2024).

### Question 4: UK House Price Index Time Series Analysis
* **Objective:** Analyze long-term residential housing dynamics in the United Kingdom.
* **Methodology:** 12-month rolling moving averages, historical phase decomposition, year-on-year percentage change, Autocorrelation Function (ACF) with Bartlett $95\%$ significance bounds, and pre- vs. post-2008 Compound Annual Growth Rate (CAGR).
* **Data Source:** Nationwide Building Society (`Monthly.xlsx`).

### Question 5: UK Real Estate vs. FTSE 100 Equities (1991–2026)
* **Objective:** Compare capital performance between residential property and equities over a 35-year horizon.
* **Methodology:** Dual-index base normalization ($1991 = 100$), Geometric CAGR vs. Arithmetic Mean returns, annualized monthly volatility ($\sigma \times \sqrt{12}$), and total return evaluation (dividends, rental yields, leverage, liquidity, and frictional costs).
* **Data Source:** `FTSE100.csv` and Nationwide House Price Index.

---

## File Structure

```text
├── nalain_DIAML_Assignment3.ipynb     # Main computational notebook (modular subquestion cells)
├── michelson_speed_of_light.json      # Dataset for Question 1
├── chickwts_casein_soybean.csv        # Dataset for Question 2
├── Monthly.xlsx                       # Dataset for Question 4
├── FTSE100.csv                        # Dataset for Question 5
└── README.md                          # Project overview and documentation
```

---

## Instructions for Execution

1. Open `nalain_DIAML_Assignment3.ipynb` in VS Code or JupyterLab.
2. Ensure dependencies are installed:
   ```bash
   pip install numpy pandas scipy matplotlib openpyxl
   ```
3. Run cells sequentially to reproduce statistical metrics and figures.
