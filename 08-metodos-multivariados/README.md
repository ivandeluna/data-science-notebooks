# 08 — Métodos Multivariados

> Dimensionality reduction and latent structure analysis applied to Mexican state-level data from INEGI and CONAPO.

---

## Notebooks

### `multivariate-eda-pca-household-consumption.ipynb`
**Multivariate EDA and PCA: Household Consumption Patterns in Mexico**

PCA applied to ENIGH household goods and services data across Mexico's 32 states.

- Exploratory analysis of 11 variables (internet, TV, appliances, AC, etc.)
- Correlation matrix and KMO test (overall KMO = 0.81 — Good)
- Component selection: cumulative variance (78.9% with 2 PCs), scree plot, Kaiser rule
- Biplot: states and variables in the same 2D space
- **Key result:** PC1 (62.8%) captures a general development axis — Chiapas/Oaxaca/Guerrero vs. Nuevo León/Baja California. PC2 (16.1%) isolates climate effects (air conditioning) vs. legacy technology (radio).

**Data:** `Hogares_equipo.xlsx` — ENIGH (INEGI), 32 states × 11 household goods/services

---

### `factor-analysis-marginalization-mexico.ipynb`
**Factor Analysis: Building a Marginalization Index for Mexico**

Factor Analysis applied to CONAPO's 9 marginalization indicators to construct a composite deprivation score.

- Normality tests (Shapiro-Wilk) for all 9 indicators
- Adequacy tests: Bartlett sphericity (p ≈ 0) and KMO (0.89 — Good)
- Single-factor solution explaining 71% of total variance
- Factor loadings and communalities — illiteracy and no primary school load highest
- Rotation methods: Varimax and Promax (identical with 1 factor — explained in notebook)
- Factor scores: state ranking from most to least marginalized
- **Key result:** Guerrero (+2.6), Chiapas (+2.4), Oaxaca (+2.2) are most marginalized; CDMX (−1.5) and Nuevo León (−1.4) are least

**Data:** `pobreza.xlsx` — CONAPO marginalization indicators by state

---

## Requirements

```
Python >= 3.9
numpy · pandas · matplotlib · seaborn · scikit-learn · scipy · factor_analyzer · openpyxl
```

```bash
pip install numpy pandas matplotlib seaborn scikit-learn scipy factor_analyzer openpyxl
```

## Data Sources

- [ENIGH 2022 — INEGI](https://www.inegi.org.mx/programas/enigh/nc/2022/) — household goods survey
- [CONAPO](https://www.gob.mx/conapo) — marginalization index indicators

## Author

**Iván de Luna** · [@ivandeluna](https://github.com/ivandeluna) · [ivandeluna.github.io](https://ivandeluna.github.io)
