<!-- BANNER -->
<div align="center">

```
████████╗███████╗██████╗ ██████╗  ██████╗ ██████╗     ██╗███████╗███╗   ███╗
╚══██╔══╝██╔════╝██╔══██╗██╔══██╗██╔═══██╗██╔══██╗    ██║╚══███╔╝████╗ ████║
   ██║   █████╗  ██████╔╝██████╔╝██║   ██║██████╔╝    ██║  ███╔╝ ██╔████╔██║
   ██║   ██╔══╝  ██╔══██╗██╔══██╗██║   ██║██╔══██╗    ██║ ███╔╝  ██║╚██╔╝██║
   ██║   ███████╗██║  ██║██║  ██║╚██████╔╝██║  ██║    ██║███████╗██║ ╚═╝ ██║
   ╚═╝   ╚══════╝╚═╝  ╚═╝╚═╝  ╚═╝ ╚═════╝ ╚═╝  ╚═╝    ╚═╝╚══════╝╚═╝     ╚═╝
```

# 🌐 Global Terrorism: A Multi-Dimensional Statistical Investigation

### *An MSc-Level End-to-End Analytical Framework spanning Descriptive Statistics, Machine Learning, Bayesian Inference, Causal Analysis, and Spatial-Network Modelling*

---

![Python](https://img.shields.io/badge/Python-3.10%2B-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebooks-F37626?style=for-the-badge&logo=jupyter&logoColor=white)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-ML%20Pipeline-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458?style=for-the-badge&logo=pandas&logoColor=white)
![Plotly](https://img.shields.io/badge/Plotly-Interactive%20Viz-3F4F75?style=for-the-badge&logo=plotly&logoColor=white)
![HuggingFace](https://img.shields.io/badge/🤗%20HuggingFace-Dataset-FFD21E?style=for-the-badge)
![Kaggle](https://img.shields.io/badge/Kaggle-Dataset-20BEFF?style=for-the-badge&logo=kaggle&logoColor=white)

</div>

---

> *"In the age of data, silence is complicity. This project speaks."*

This repository is the complete analytical artefact of an **MSc-level capstone investigation** into global terrorism — combining **three decades of incident data**, **socio-economic indicators**, and **governance metrics** into a single, rigorous, reproducible research pipeline. From raw CSV to calibrated Gradient Boosting classifiers, from chi-squared tests to Bayesian posterior distributions, from regional dashboards to network graphs of attack patterns — every layer of modern statistical science is brought to bear on one of humanity's most consequential problems.

---

## 🗂️ Table of Contents

- [The Research Question](#-the-research-question)
- [Project Architecture](#-project-architecture)
- [Datasets & Sources](#-datasets--sources)
- [Analytical Notebooks — The Full Pipeline](#-analytical-notebooks--the-full-pipeline)
  - [GTD Core Analysis (NB1–NB10)](#gtd-core-analysis-nb1nb10)
  - [Socio-Economic & Governance Analysis](#socio-economic--governance-analysis)
  - [Rough Exploration Notebooks](#rough-exploration-notebooks)
- [Technologies & Stack](#-technologies--stack)
- [Key Outputs & Visuals](#-key-outputs--visuals)
- [How to Run](#-how-to-run)
- [Data Access](#-data-access)

---

## ❓ The Research Question

> **What structural, socio-economic, and governance-level factors determine whether a terrorist attack succeeds — and how many casualties it inflicts?**

This project unpacks terrorism not as isolated incidents, but as a **systemic phenomenon** shaped by GDP per capita, government effectiveness, political stability, urbanisation, and historical attack patterns. Using the **Global Terrorism Database (GTD)** fused with **World Bank Socio-Economic indicators** and **Worldwide Governance Indicators (WGI)**, the analysis spans:

- 🔴 **Attack success prediction** (binary classification)
- 💀 **Fatality modelling** (regression & count models)
- 🌍 **Geographic clustering** of violence hotspots
- 📈 **Temporal forecasting** of terrorism trends
- 🧠 **Causal inference** — what *causes* attacks to be lethal?
- 🕸️ **Network graphs** — how do terrorist groups and tactics interconnect?

---

## 🏗️ Project Architecture

```
Terrorism_repo/
│
├── 📂 data/
│   ├── raw/                    ← Original unprocessed datasets (not tracked; see links below)
│   ├── panel_data/             ← Cleaned, merged panel datasets
│   └── sample/                 ← Sample notebooks for quick data exploration
│       ├── gtd.ipynb
│       ├── socio_economic.ipynb
│       └── wgi.ipynb
│
├── 📂 GTD FINAL ANALYSIS/      ← 🔥 Core analytical pipeline (NB1–NB10)
│   ├── NB1_Descriptive_EDA.ipynb
│   ├── NB2_Inferential_Statistics.ipynb
│   ├── NB3_Regression_Success.ipynb
│   ├── NB4_Regression_Fatality.ipynb
│   ├── NB5_Combined_Models.ipynb
│   ├── NB6_Machine_Learning.ipynb
│   ├── NB7_Advanced_Statistical_DS.ipynb
│   ├── NB8_Bayesian_Causal.ipynb
│   ├── NB9_Spatial_Network_Features.ipynb
│   └── NB10_Capstone_Synthesis.ipynb  ← 🎓 Capstone: Full Pipeline + Research Synthesis
│
├── 📂 SOCIO_WGI FINAL ANALYSIS/  ← Merged multi-source panel analysis
│   ├── 01_data_loading_and_eda.ipynb
│   ├── 02_feature_engineering.ipynb
│   ├── 03_ols_assumptions.ipynb
│   ├── 04_ridge_lasso.ipynb
│   ├── 05_model_comparison.ipynb
│   ├── 06_advanced_models.ipynb
│   └── Terrorism_Complete_End_to_End.ipynb  ← Single-file mega-notebook
│
├── 📂 notebooks_rough_analysis/  ← Exploratory / ideation notebooks
│   ├── gtd/
│   ├── socio_economic/
│   ├── wgi/
│   └── merged/
│
├── 📂 outputs/
│   ├── animations/             ← World heatmap GIFs, attack evolution over time
│   ├── dashboards/             ← Regional dashboards (Africa, Asia, Europe, Americas, Aus)
│   ├── tables/                 ← Research gap analysis tables
│   └── reports/
│
├── 📂 END SEM/
│   ├── DarkPulse.html          ← Interactive dark-themed analytics dashboard
│   ├── DarkTrace.html          ← Attack tracing visualisation
│   └── Application_Cases_Tables.docx
│
├── 📂 docs/
│   └── Codebook.pdf            ← GTD variable codebook
│
└── 📂 Visuals/
    └── Animation.ipynb         ← Animated cartographic visualisations
```

---

## 📦 Datasets & Sources

This project fuses **three independent data sources** into a unified panel dataset covering **180+ countries across 30+ years**.

| Dataset | Description | Source |
|---|---|---|
| **Global Terrorism Database (GTD)** | 200,000+ terrorist incidents: attack type, weapon, target, group, casualties, success | [START / UMD](https://www.start.umd.edu/gtd/) |
| **World Bank Socio-Economic Indicators** | GDP per capita, urbanisation, unemployment, population density, inequality | [World Bank Open Data](https://data.worldbank.org/) |
| **Worldwide Governance Indicators (WGI)** | Rule of law, political stability, govt effectiveness, control of corruption, voice & accountability | [World Bank WGI](https://info.worldbank.org/governance/wgi/) |

### 🔗 Full Dataset Access

Due to file size constraints, the complete datasets are hosted externally:

- 🟠 **Kaggle:** [terrorism-socio-economic-and-governance-dataset](https://www.kaggle.com/datasets/tanyatanu1403/terrorism-socio-economic-and-governance-dataset)
- 🤗 **Hugging Face:** [tanu14/Terrorism](https://huggingface.co/datasets/tanu14/Terrorism)

---

## 📓 Analytical Notebooks — The Full Pipeline

### GTD Core Analysis (NB1–NB10)

Each notebook is a **self-contained analytical chapter**, designed to be read in sequence. Together they form a complete MSc-grade research narrative.

---

#### `NB1` — Descriptive & Exploratory Statistics
> *"Before inference, there must be understanding."*

Establishes the statistical portrait of the GTD: univariate summaries, frequency analyses, distribution characterisation (skewness, kurtosis, Pareto principle in violence), temporal decomposition, geographic heatmaps, and bivariate exploration. The Pareto principle turns out to hold dramatically — a handful of groups and regions account for the overwhelming majority of casualties.

**Skills demonstrated:** Distributional analysis, missingness patterns, time-series decomposition, geographic profiling, cross-tabulation.

---

#### `NB2` — Inferential Statistics
> *"Does it differ, or is it noise?"*

Parametric and non-parametric hypothesis tests assess whether terrorism patterns differ meaningfully across attack types, regions, and time periods. Every test is chosen with rigour — assumptions checked, effect sizes reported alongside p-values.

**Tests covered:** χ² independence · Fisher's exact (2×2) · One-way ANOVA · Welch's t-test · Kruskal-Wallis · Mann-Whitney U · Kolmogorov-Smirnov

---

#### `NB3` — Regression: Attack Success
> *"What makes an attack succeed?"*

Binary regression models (logistic, probit) predict whether an attack achieves its tactical objective. Features include attack type, weapon choice, target category, group affiliation, and country-level controls. Odds ratios are interpreted substantively.

---

#### `NB4` — Regression: Fatality Modelling
> *"What drives casualties?"*

OLS and count models (Poisson, Negative Binomial) model the number of fatalities per incident. Zero-inflated models address the preponderance of low-casualty events. The relationship between attack sophistication and lethality is quantified.

---

#### `NB5` — Combined Models
> *"Pulling the threads together."*

Combines success and fatality models, exploring interaction effects between socio-economic context and attack characteristics. Panel fixed-effects regressions account for country-level unobserved heterogeneity.

---

#### `NB6` — End-to-End Machine Learning Pipeline
> *"From raw features to calibrated predictions."*

A production-quality sklearn `Pipeline` with preprocessing, feature engineering, model selection, hyperparameter tuning, and ensemble methods. Full evaluation suite: ROC-AUC, precision-recall, calibration curves, learning curves.

**Models trained:** Decision Tree · Random Forest · Extra Trees · Gradient Boosting · SVM · MLP (Neural Net) · Logistic Regression · Gaussian Naive Bayes · Isolation Forest (anomaly)

**Best model:** Calibrated Gradient Boosting Classifier (isotonic regression calibration)

---

#### `NB7` — Advanced Statistical & Data Science Applications
> *"Where statistics meets data science."*

Goes beyond standard modelling into clustering, dimensionality reduction, anomaly detection, and survival analysis.

**Techniques:** K-Means clustering · Hierarchical clustering (Ward linkage, dendrogram) · DBSCAN · PCA · t-SNE · FastICA · NMF · Isolation Forest · Mutual Information feature selection · RFE

---

#### `NB8` — Bayesian Statistics, Probabilistic Modelling & Causal Inference
> *"Not just 'is there a difference?' — but 'how certain are we, and why?'"*

The most theoretically demanding notebook. Replaces frequentist point estimates with full posterior distributions. Causal DAGs encode domain assumptions; propensity score matching and difference-in-differences estimate treatment effects.

**Techniques:**
- Bayesian A/B testing (Beta-Binomial conjugate model)
- Naive Bayes classifier with posterior analysis
- Bayesian update simulation
- Propensity Score Matching (PSM)
- Difference-in-Differences (DiD)
- Directed Acyclic Graphs (DAGs) for causal assumptions

---

#### `NB9` — Spatial Analysis, Network Graphs & Advanced Feature Engineering
> *"Violence has geography. Violence has networks."*

Extracts spatial intelligence from geographic coordinates. Builds network representations of terrorism: nodes are groups, edges are shared tactics or co-occurring attacks. Advanced feature engineering captures temporal dynamics and group-level behaviour.

**Techniques:** Haversine distance matrices · DBSCAN spatial clustering · NetworkX graph construction · Betweenness centrality · PageRank · Temporal lag features · Rolling attack-rate windows

---

#### `NB10` — Capstone: Full Pipeline, Explainability, Forecasting & Research Synthesis
> *"The final word."*

Integrates every preceding analysis into a single production pipeline. Adds model interpretability (permutation importance, partial dependence plots, SHAP-style local attribution) and temporal forecasting (Holt-Winters, ARIMA-style decomposition). Ends with a formal research synthesis and implications for policy.

**Sections:** Production sklearn Pipeline · Global & local feature attribution · Partial dependence · Forecasting · Calibration · Research synthesis

---

### Socio-Economic & Governance Analysis

Located in `SOCIO_WGI FINAL ANALYSIS/` — a parallel analytical track that focuses on the **macro-level drivers** of terrorism by merging GTD incident data with WGI and socio-economic panel data.

| Notebook | Focus |
|---|---|
| `01_data_loading_and_eda.ipynb` | Panel data construction, missingness, exploratory profiling |
| `02_feature_engineering.ipynb` | Lag features, interaction terms, governance composite indices |
| `03_ols_assumptions.ipynb` | Full OLS assumption testing: linearity, homoscedasticity, normality, multicollinearity (VIF) |
| `04_ridge_lasso.ipynb` | Regularised regression for high-dimensional governance + socio-economic feature sets |
| `05_model_comparison.ipynb` | AIC/BIC model selection, cross-validated RMSE comparison |
| `06_advanced_models.ipynb` | Random Forest, GBM, and ensemble models on the merged panel |
| `Terrorism_Complete_End_to_End.ipynb` | 🏆 Single mega-notebook: entire SOCIO_WGI pipeline from raw data to final model |

---

### Rough Exploration Notebooks

`notebooks_rough_analysis/` contains the **ideation and exploration** work — GDP vs Terror visualisations, panel data experiments, WGI correlation studies, fatality rate analyses. This is where the research hypotheses were born.

---

## 🛠️ Technologies & Stack

### Core Scientific Stack

| Library | Version | Purpose |
|---|---|---|
| `Python` | 3.10+ | Core language |
| `pandas` | Latest | Data manipulation, panel merging, group-by aggregations |
| `numpy` | Latest | Numerical computation, matrix operations |
| `scipy` | Latest | Statistical tests (chi2, ANOVA, KS, Fisher, t-test), distributions |
| `matplotlib` | Latest | Base plotting, gridspec layouts, custom styling |
| `seaborn` | Latest | Statistical visualisation, heatmaps, pairplots, violin plots |

### Machine Learning

| Library | Purpose |
|---|---|
| `scikit-learn` | Full ML pipeline — preprocessing, model selection, evaluation, feature importance |
| `sklearn.ensemble` | RandomForest, GradientBoosting, ExtraTrees, IsolationForest |
| `sklearn.svm` | Support Vector Classifier |
| `sklearn.neural_network` | MLPClassifier |
| `sklearn.cluster` | KMeans, AgglomerativeClustering, DBSCAN |
| `sklearn.decomposition` | PCA, FastICA, NMF |
| `sklearn.manifold` | t-SNE |
| `sklearn.calibration` | CalibratedClassifierCV, calibration curves |
| `sklearn.inspection` | Permutation importance, partial dependence |
| `sklearn.feature_selection` | Mutual info, RFE, SelectFromModel |
| `sklearn.pipeline` | Pipeline, ColumnTransformer |

### Statistics & Inference

| Library | Purpose |
|---|---|
| `scipy.stats` | Hypothesis tests, distributions (Beta, Gamma, Binomial, Dirichlet, Normal) |
| `scipy.cluster.hierarchy` | Hierarchical clustering, dendrograms |
| `scipy.special` | `betaln` for Bayesian log-likelihood |
| `scipy.signal` | Peak detection in time series |
| `statsmodels` | OLS with full diagnostics, VIF, ACF/PACF, panel models |

### Spatial & Network

| Library | Purpose |
|---|---|
| `networkx` | Graph construction, centrality measures, community detection |
| `scipy.spatial` | Haversine/cdist distance matrices |
| `sklearn.cluster.DBSCAN` | Spatial density clustering |

### Visualisation & Interactivity

| Library | Purpose |
|---|---|
| `plotly` | Interactive choropleth maps, animated scatter plots, sunburst charts |
| `folium` | Leaflet.js-powered interactive maps |
| `matplotlib` | Publication-quality static figures |
| `seaborn` | Statistical graphics |

### Data & Reproducibility

| Tool | Purpose |
|---|---|
| `Jupyter Notebook` | Interactive narrative computing |
| `Kaggle Datasets` | Full dataset hosting |
| `Hugging Face Datasets` | Model/dataset hub |
| `Git LFS` | Large file storage for datasets |
| `openpyxl` | Excel panel data I/O |

---

## 🖼️ Key Outputs & Visuals

| Output | Description |
|---|---|
| `outputs/animations/world_heatmap.png` | Global terrorism intensity heatmap |
| `outputs/animations/over_the_years.png` | Evolution of attacks 1970–2020 |
| `outputs/dashboards/africa.png` | Africa regional terrorism dashboard |
| `outputs/dashboards/asia.png` | Asia regional terrorism dashboard |
| `outputs/dashboards/europe.png` | Europe regional terrorism dashboard |
| `outputs/dashboards/north_america.png` | North America dashboard |
| `outputs/dashboards/south_america.png` | South America dashboard |
| `outputs/dashboards/australia.png` | Australia/Oceania dashboard |
| `outputs/tables/research_gap.png` | Visualised research gap analysis |
| `END SEM/DarkPulse.html` | 🌑 Interactive dark-themed analytics dashboard |
| `END SEM/DarkTrace.html` | Interactive attack tracing visualisation |

---

## 🚀 How to Run

### 1. Clone the repository

```bash
git clone https://github.com/YOUR_USERNAME/terrorism-analysis.git
cd terrorism-analysis
```

### 2. Install dependencies

```bash
pip install pandas numpy scipy matplotlib seaborn scikit-learn statsmodels \
            networkx plotly folium openpyxl jupyter
```

### 3. Download the data

Place datasets in `data/raw/` after downloading from:
- 🟠 [Kaggle](https://www.kaggle.com/datasets/tanyatanu1403/terrorism-socio-economic-and-governance-dataset)
- 🤗 [Hugging Face](https://huggingface.co/datasets/tanu14/Terrorism)

### 4. Run in order

**GTD Analysis:**
```
GTD FINAL ANALYSIS/NB1 → NB2 → NB3 → NB4 → NB5 → NB6 → NB7 → NB8 → NB9 → NB10
```

**Socio-WGI Analysis:**
```
SOCIO_WGI FINAL ANALYSIS/01 → 02 → 03 → 04 → 05 → 06
```

Or run the single end-to-end mega-notebook:
```
SOCIO_WGI FINAL ANALYSIS/Terrorism_Complete_End_to_End.ipynb
```

---

## 📌 Notes

- Sample datasets in `data/sample/` allow quick testing without the full download
- All notebooks use `warnings.filterwarnings('ignore')` for clean output — disable this during development
- Git LFS is configured for large binary files

---

<div align="center">

---

*Built with rigour. Driven by curiosity. Dedicated to understanding.*

**MSc Data Science Capstone Project** · Global Terrorism Database Analysis

---

</div>
