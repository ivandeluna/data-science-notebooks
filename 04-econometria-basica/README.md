# 04 — Econometría Básica

> Regression, causal inference, and treatment effect estimation using real Mexican household data.

---

## Notebooks

### `linear_regression_lasso_ridge.ipynb`
**Linear Regression, Lasso, and Ridge: Predicting Household Income in Mexico**

End-to-end regression workflow using ENIGH 2022 data (91,414 households).

- OLS regression with economic interpretation of coefficients
- Outlier treatment with winsorization (raises R² from 0.28 to 0.53)
- Regularization: Lasso with cross-validated λ selection (LassoCV), Ridge regression
- Coefficient comparison across three models
- **Key result:** Education adds ~$2,400 MXN/month per year of schooling; gender gap persists at ~$4,100 MXN/month after controls

**Data:** `concentradohogar.csv` — ENIGH 2022 (INEGI), 91,414 households, 126 variables

---

### `rct_difference_in_differences.ipynb`
**Power Analysis and Difference-in-Differences: Causal Inference from Observational Data**

Two complementary tools for causal inference:

- Statistical power analysis: minimum sample size, power curves, effect size trade-offs
- Difference-in-Differences (DiD): manual calculation and regression-based estimation
- Counterfactual visualization: what would have happened without treatment?
- Parallel trends assumption and its interpretation

---

## Requirements

```
Python >= 3.9
numpy · pandas · matplotlib · seaborn · scikit-learn · statsmodels
```

```bash
pip install numpy pandas matplotlib seaborn scikit-learn statsmodels
```

## Data Sources

- [ENIGH 2022 — INEGI](https://www.inegi.org.mx/programas/enigh/nc/2022/) — `concentradohogar.csv` included in this folder

## Author

**Iván de Luna** · [@ivandeluna](https://github.com/ivandeluna) · [ivandeluna.github.io](https://ivandeluna.github.io)
