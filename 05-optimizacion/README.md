# 05 — Optimización Estocástica

> From-scratch implementation of four stochastic optimization algorithms, benchmarked on classic test functions.

---

## Notebooks

### `optimizacion-estocastica-python.qmd`
**Stochastic Optimization with Python: Random Search, Differential Evolution, PSO, and SGD**

Four algorithms implemented without optimization libraries, compared on three benchmark functions.

- **Random Search** — pure exploration baseline; O(T·n) complexity
- **Differential Evolution (DE/Rand/1/bin)** — population-based with directional mutation
- **PSO** — swarm intelligence with personal and neighborhood memory
- **SGD** — stochastic gradient descent for data-driven learning

Benchmark functions: Rastrigin (highly multimodal), Ackley (single global minimum), Custom (non-separable)

Published as a tutorial post at [ivandeluna.github.io](https://ivandeluna.github.io)

---

## Requirements

```
Python >= 3.9
numpy · matplotlib · pandas · scikit-learn
```

```bash
pip install numpy matplotlib pandas scikit-learn
```

> **Note:** This notebook is a `.qmd` file (Quarto Markdown). To run it as a standard notebook, rename to `.ipynb` or open with Quarto.

## Author

**Iván de Luna** · [@ivandeluna](https://github.com/ivandeluna) · [ivandeluna.github.io](https://ivandeluna.github.io)
