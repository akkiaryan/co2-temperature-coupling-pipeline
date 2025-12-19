# CO₂–Temperature Coupling Pipeline

![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)
![Python](https://img.shields.io/badge/Python-3.9+-3776AB?logo=python&logoColor=white)
![pandas](https://img.shields.io/badge/pandas-Data%20Analysis-150458?logo=pandas)
![statsmodels](https://img.shields.io/badge/statsmodels-Time%20Series-4B8BBE)
![Prophet](https://img.shields.io/badge/Prophet-Forecasting-black)
![GitHub](https://img.shields.io/badge/GitHub-Reproducible%20Research-181717?logo=github)

A country-resolved computational framework for analyzing the coupling between carbon dioxide (CO₂) emissions and surface temperature using causality testing and time-series forecasting models.

---

## Conference Context
This work was **presented at the 3rd International Conference on Nanoscience and Nanotechnology (ICNAN 2025)**  
**Vellore Institute of Technology (VIT), Vellore, India**  
**16–19 December 2025**

The project was evaluated in a peer-reviewed academic setting, with emphasis on scientific rigor, reproducibility, and methodological clarity.

---

## Authors & Contributors
- **Akki Aryan** — System conception, pipeline architecture, data engineering, modeling, analysis, visualization  
- **Prateek Kumar** — Data preprocessing assistance, exploratory validation, result verification  
- **Dr. Nalini N** — Academic supervision and guidance  

Affiliation:  
School of Computer Science and Engineering (SCOPE),  
Vellore Institute of Technology, Vellore, India

---

## Abstract
Carbon dioxide plays a fundamental role in Earth’s carbon cycle and radiative balance, influencing climate dynamics across molecular, nanoscale, and planetary regimes. While global-average analyses dominate climate modeling literature, such aggregation often obscures regional heterogeneity and directional dependencies between emissions and temperature.

This project presents a **country-resolved computational pipeline** for analyzing CO₂–temperature coupling using statistically grounded time-series methods. The pipeline integrates multi-source emissions and temperature datasets, performs rigorous preprocessing and temporal alignment, applies Granger causality testing and VAR/VARX models to examine directional influence, and generates interpretable forecasts using ARIMA-based methods and Prophet.

By shifting from global averages to country-level analysis, the framework reveals heterogeneous causal structures and temporal dynamics, offering a reproducible foundation for climate-system modeling and carbon-cycle interpretation.

---

## Motivation
Carbon is the backbone of the ecosystem we inhabit. At the nanoscale, carbon-based interactions govern energy absorption and emission; at the macroscale, aggregated anthropogenic emissions alter atmospheric composition and temperature dynamics.

Most climate studies emphasize correlation at global scale. This project was motivated by the need to:
- Resolve CO₂–temperature relationships **at the country level**
- Distinguish **directional causality** from correlation
- Build a **transparent, reproducible computational pipeline** suitable for scientific evaluation and forecasting

---

## Project Objectives
- Integrate multi-source CO₂ emissions and temperature datasets
- Perform statistically rigorous preprocessing and temporal alignment
- Test causal relationships using econometric time-series models
- Generate interpretable forecasts of CO₂ and temperature trends

---

## Working of the Pipeline

### 1. Data Acquisition
- CO₂ emissions data from **Our World in Data**
- Surface temperature anomalies from **NASA GISTEMP**
- Optional socio-economic covariates (GDP, population) as exogenous drivers

All datasets are standardized to a **yearly, country-resolved format**.

---

### 2. Preprocessing & Alignment
- Time-series aware missing-value interpolation
- Country code standardization
- Year-wise temporal alignment across sources
- Preparation for stationarity-sensitive modeling

---

### 3. Causality Analysis
- **Granger causality tests** for directional dependency
- **VAR and VARX models** for multivariate temporal dynamics
- Lag structure selection based on stability and information criteria

---

### 4. Forecasting
- **ARIMA / SARIMA** statistical baselines
- **Prophet** for trend and long-horizon forecasting
- Comparative evaluation across models

---

### 5. Analysis & Visualization
- Country-wise diagnostics and plots
- Interpretation of causal strength and coefficients
- Preparation of conference-ready figures

---

## Development Timeline (4 Months)

**Total duration:** ~4 months (research-driven, iterative)

### Month 1 — Problem Formulation & Literature Review
- Study of IPCC AR6 and Global Carbon Budget reports
- Identification of limitations in global-average modeling
- Framing of country-resolved causality as core contribution

---

### Month 2 — Data Acquisition & Preprocessing
- Collection of emissions and temperature datasets
- Country and temporal standardization
- Missing-value handling and validation
- Initial exploratory data analysis

---

### Month 3 — Modeling & Causality Analysis
- Implementation of Granger causality testing
- VAR and VARX model development
- Lag sensitivity and stability analysis
- Intermediate validation and refinement

---

### Month 4 — Forecasting, Analysis & Packaging
- ARIMA and Prophet forecasting
- Comparative evaluation and visualization
- Interpretation of results
- Documentation, release preparation, and conference submission

---

## Technology Stack

### Core Language
- **Python 3.9+**

### Data & Analysis
- pandas, numpy
- statsmodels (VAR, VARX, Granger causality)

### Forecasting
- ARIMA / SARIMA
- Prophet

### Visualization
- matplotlib

### Reproducibility & Tooling
- GitHub (version control and releases)
- Google Colab (execution environment)

---

## Outputs
- Cleaned, country-resolved datasets
- Causality metrics and diagnostics
- Forecast projections for CO₂ and temperature
- Conference-ready figures and artifacts

---

## Reproducibility
The pipeline is designed for reproducible execution using scripts and notebooks. All preprocessing, modeling, and analysis steps are documented within the repository.

---

## License
This project is released under the **MIT License**.  
You are free to use, modify, and distribute this work with appropriate attribution.

---

## Reference
This repository corresponds to the work presented at ICNAN 2025:

**“Beyond Global Averages: A Country-Resolved Pipeline for CO₂–Temperature Coupling, Causality Testing, and Forecasting.”**
