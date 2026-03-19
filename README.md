# data-science-notebooks

> Quantitative economics and data science tutorials — implemented from scratch in Python, applied to real Mexican datasets.

**Iván de Luna** · [@ivandeluna](https://github.com/ivandeluna) · [ivandeluna.github.io](https://ivandeluna.github.io)

---

## About

This repository contains self-contained tutorial notebooks covering statistics, econometrics, machine learning, and optimization — built with real data from INEGI, CONAPO, and other Mexican sources. Each notebook includes theory, implementation, and interpretation, with no assumed prior knowledge beyond basic Python.

---

## Contents

| Folder | Topic | Notebooks |
|--------|-------|-----------|
| [`04-econometria-basica`](04-econometria-basica/) | Econometrics | Linear regression with Lasso & Ridge · RCT & Difference-in-Differences |
| [`05-optimizacion`](05-optimizacion/) | Stochastic Optimization | Random Search · Differential Evolution · PSO · SGD |
| [`08-metodos-multivariados`](08-metodos-multivariados/) | Multivariate Methods | Multivariate EDA & PCA · Factor Analysis |

---

## Requirements

All notebooks use Python 3.9+. Install dependencies with:

```bash
pip install numpy pandas matplotlib seaborn scikit-learn statsmodels factor_analyzer openpyxl
```

---

## Data

Real datasets used across notebooks:

| Dataset | Source | Used in |
|---------|--------|---------|
| ENIGH 2022 — `concentradohogar.csv` | [INEGI](https://www.inegi.org.mx/programas/enigh/nc/2022/) | `04-econometria-basica` |
| Household goods by state — `Hogares_equipo.xlsx` | ENIGH / INEGI | `08-metodos-multivariados` |
| CONAPO marginalization indicators — `pobreza.xlsx` | [CONAPO](https://www.gob.mx/conapo) | `08-metodos-multivariados` |

---

## Author

**Iván de Luna** — Quantitative economist. Focus on regional development in Mexico.

- GitHub: [@ivandeluna](https://github.com/ivandeluna)
- Site: [ivandeluna.github.io](https://ivandeluna.github.io)
- Research: DAAD — Doctorado en Administración y Alta Dirección
