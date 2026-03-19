# 04 — Econometría Básica / Basic Econometrics

Notebooks covering fundamental econometric methods, with emphasis on causal inference, experimental design, and regularized regression. All notebooks are self-contained: theory is introduced before code, and results are interpreted in context.

---

## Notebooks

### 1. `rct_difference_in_differences.ipynb`
**RCT Design & Difference-in-Differences Estimation**

Covers the two core stages of a Randomized Controlled Trial:
- **Statistical power analysis** — determining minimum sample size before collecting data (with cross-validated visualizations of power vs. effect size)
- **Difference-in-Differences (DiD)** — estimating causal treatment effects via manual calculation, OLS regression, and the counterfactual visualization

Topics: `causal-inference` · `rct` · `difference-in-differences` · `statistical-power` · `statsmodels`

---

### 2. `linear_regression_lasso_ridge.ipynb`
**Linear Regression with Regularization: OLS, Lasso (L1), and Ridge (L2)**

Applied to real Mexican household data from the **ENIGH 2022** (INEGI). Covers:
- OLS regression with multicollinearity discussion
- Lasso (L1) with automatic variable selection via cross-validated λ
- Ridge (L2) with coefficient shrinkage via cross-validated λ
- Full model comparison: coefficients, R², RMSE, and economic interpretation

**Data required:** `concentradohogar.csv` — download from [INEGI ENIGH 2022](https://www.inegi.org.mx/programas/enigh/nc/2022/#documentacion)

Topics: `regression` · `lasso` · `ridge` · `regularization` · `enigh` · `mexico` · `scikit-learn`

---

## Requirements

```bash
pip install numpy pandas matplotlib seaborn scipy statsmodels scikit-learn
```