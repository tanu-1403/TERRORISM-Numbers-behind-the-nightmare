<div align="center">

<br>

```
╔══════════════════════════════════════════════════════╗
║          G L O B A L   T E R R O R I S M            ║
║                  A N A L Y S I S                     ║
╚══════════════════════════════════════════════════════╝
```

*An end-to-end statistical investigation into the structural, socio-economic,*
*and governance drivers of terrorism*

**200,000+ incidents · 180+ countries · 50 years of data**

<br>

![Python](https://img.shields.io/badge/Python-3.10+-black?style=flat-square&logo=python&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-notebook-black?style=flat-square&logo=jupyter&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-ML-black?style=flat-square&logo=scikitlearn&logoColor=white)
![pandas](https://img.shields.io/badge/pandas-data-black?style=flat-square&logo=pandas&logoColor=white)
![License](https://img.shields.io/badge/license-MIT-black?style=flat-square)

`MSc Data Science` `Capstone Project`

<br>

</div>

---

## ❝ Research Question

> What **structural, socio-economic, and governance-level factors** determine whether
> a terrorist attack succeeds — and how many casualties it inflicts?

---

## 📦 Datasets

| Dataset | Coverage | Source |
|---|---|---|
| **Global Terrorism Database (GTD)** | 200k+ incidents · attack type, weapon, target, casualties, success · 1970–2020 | [START / UMD](https://www.start.umd.edu/gtd/) |
| **World Bank Socio-Economic** | GDP per capita, urbanisation, unemployment, population density | [World Bank Open Data](https://data.worldbank.org/) |
| **Worldwide Governance Indicators** | Rule of law, political stability, govt effectiveness, corruption control | [World Bank WGI](https://info.worldbank.org/governance/wgi/) |
| **Full merged panel** ⭐ | Complete dataset — hosted externally due to size | [Kaggle](https://www.kaggle.com/datasets/tanyatanu1403/terrorism-socio-economic-and-governance-dataset) · [Hugging Face](https://huggingface.co/datasets/tanu14/Terrorism) |

---

## 🗂 Notebook Index

### Track 1 — GTD Core Pipeline &nbsp;`GTD FINAL ANALYSIS/`

| # | Notebook | Methods |
|---|---|---|
| `NB 01` | **Descriptive & Exploratory Statistics** | Univariate summaries, Pareto analysis, temporal decomposition, geographic heatmaps |
| `NB 02` | **Inferential Statistics** | χ², Fisher's exact, ANOVA, Welch's t-test, Kruskal-Wallis, Mann-Whitney, KS — all with effect sizes |
| `NB 03` | **Regression: Attack Success** | Logistic & probit models predicting tactical success; odds ratios interpreted substantively |
| `NB 04` | **Regression: Fatality Modelling** | OLS, Poisson, Negative Binomial, zero-inflated models for casualty counts |
| `NB 05` | **Combined Models** | Interaction effects, panel fixed-effects regressions across success and fatality outcomes |
| `NB 06` | **Machine Learning Pipeline** | RandomForest, GBM, SVM, MLP, ExtraTrees, Naive Bayes · calibrated GBM wins · full ROC/PR suite |
| `NB 07` | **Advanced Statistical Methods** | K-Means, hierarchical clustering, DBSCAN, PCA, t-SNE, FastICA, NMF, Isolation Forest |
| `NB 08` | **Bayesian & Causal Inference** | Beta-Binomial posteriors, Bayesian A/B testing, DAGs, propensity score matching, DiD |
| `NB 09` | **Spatial & Network Analysis** | Haversine clustering, NetworkX graphs, betweenness centrality, PageRank, temporal lag features |
| `NB 10` ✦ | **Capstone Synthesis** | Production sklearn pipeline, SHAP-style attribution, partial dependence, temporal forecasting |

### Track 2 — Socio-Economic & Governance &nbsp;`SOCIO_WGI FINAL ANALYSIS/`

| # | Notebook | Focus |
|---|---|---|
| `01` | **Data Loading & EDA** | Panel construction, missingness profiling, exploratory statistics on merged dataset |
| `02` | **Feature Engineering** | Lag features, interaction terms, governance composite indices |
| `03` | **OLS Assumption Testing** | Linearity, homoscedasticity, normality, multicollinearity (VIF) — full Gauss-Markov check |
| `04` | **Ridge & Lasso** | Regularised regression for high-dimensional governance + socio-economic feature sets |
| `05` | **Model Comparison** | AIC/BIC selection, cross-validated RMSE, bias-variance trade-off visualisation |
| `06` | **Advanced Models** | Random Forest, GBM, ensemble methods on the merged panel dataset |

> **Shortcut:** run everything at once via `SOCIO_WGI FINAL ANALYSIS/Terrorism_Complete_End_to_End.ipynb`

---

## 🛠 Tech Stack

<table>
<tr>
<td><b>Core</b></td>
<td><code>pandas</code> <code>numpy</code> <code>scipy</code> <code>statsmodels</code></td>
</tr>
<tr>
<td><b>ML</b></td>
<td><code>scikit-learn</code> <code>Pipeline</code> <code>GBM</code> <code>SVM</code> <code>MLP</code> <code>ExtraTrees</code></td>
</tr>
<tr>
<td><b>Statistics</b></td>
<td><code>scipy.stats</code> <code>beta-binomial</code> <code>DBSCAN</code> <code>PCA</code> <code>t-SNE</code></td>
</tr>
<tr>
<td><b>Visualisation</b></td>
<td><code>plotly</code> <code>seaborn</code> <code>matplotlib</code> <code>folium</code></td>
</tr>
<tr>
<td><b>Spatial / Graph</b></td>
<td><code>networkx</code> <code>haversine</code> <code>geopandas</code></td>
</tr>
<tr>
<td><b>Reproducibility</b></td>
<td><code>Jupyter</code> <code>Git LFS</code> <code>Kaggle</code> <code>HuggingFace</code></td>
</tr>
</table>

---

## 📊 Outputs

| Output | Description |
|---|---|
| 🗺 **World heatmap** | Global terrorism intensity, animated over decades |
| 📈 **Regional dashboards** | Africa, Asia, Europe, Americas, Australia |
| 🖥 **DarkPulse.html** | Interactive dark-themed analytics dashboard |
| 🕸 **Network graphs** | Group–tactic co-occurrence and centrality analysis |
| 📋 **Research gap table** | Visualised literature positioning |
| 📄 **Capstone report** | Full model synthesis and policy implications |

---

## 🚀 Getting Started

**1 · Clone & install**

```bash
git clone https://github.com/YOUR_USERNAME/terrorism-analysis.git
cd terrorism-analysis

pip install pandas numpy scipy matplotlib seaborn scikit-learn \
            statsmodels networkx plotly folium openpyxl jupyter
```

**2 · Download the data**

Fetch from [Kaggle](https://www.kaggle.com/datasets/tanyatanu1403/terrorism-socio-economic-and-governance-dataset) or [Hugging Face](https://huggingface.co/datasets/tanu14/Terrorism) and place all files in `data/raw/`.

**3 · Run GTD notebooks in order**

```
GTD FINAL ANALYSIS/
  NB1 → NB2 → NB3 → NB4 → NB5 → NB6 → NB7 → NB8 → NB9 → NB10
```

**4 · Or run the single mega-notebook**

```
SOCIO_WGI FINAL ANALYSIS/Terrorism_Complete_End_to_End.ipynb
```

---

<div align="center">

*Built with rigour · driven by curiosity · MSc Data Science Capstone*

[Kaggle](https://www.kaggle.com/datasets/tanyatanu1403/terrorism-socio-economic-and-governance-dataset) &nbsp;·&nbsp; [Hugging Face](https://huggingface.co/datasets/tanu14/Terrorism)

</div>
