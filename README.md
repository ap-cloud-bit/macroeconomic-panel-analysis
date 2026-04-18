# 🌍 Global Macroeconomic Panel Analysis
## Real Interest Rates, Economic Crises, and Unemployment

### 📊 A Cross‑Country Panel Data Study

---

## 📌 Project Overview

This project investigates the relationship between **real interest rates and unemployment** using a **global panel dataset** covering multiple countries over several decades. The analysis focuses on three central research questions:

1. How are real interest rates associated with unemployment across countries?
2. Do monetary policy effects on unemployment occur with a delay?
3. Do major global crises—specifically the **2008 Global Financial Crisis** and the **2020 COVID‑19 pandemic**—alter unemployment dynamics or monetary transmission?

To address these questions, the project combines **descriptive analysis**, **fixed‑effects panel regressions**, and **crisis‑based robustness checks**. The objective is not only to estimate statistical relationships, but also to develop an interpretable and policy‑relevant narrative around global labor markets.

---

## 📁 Repository Structure

```text
macroeconomic-panel-analysis/
│
├── notebooks/
│   ├── 01_data_cleaning_and_merging.ipynb
│   └── 02_analysis_and_regression.ipynb
│
├── data/
│   └── processed/
│       └── final_panel_dataset.csv
│
├── figures/
│   └── (optional: saved plots)
│
├── README.md
└── requirements.txt

```
---

## 📓 **Project Notebook**
The analysis is organized into two Jupyter notebooks, each with a clear and distinct purpose.

1️⃣ Data Cleaning and Merging
Path: notebooks/01_data_cleaning_and_merging.ipynb
This notebook covers:

Loading data from multiple macroeconomic sources
Cleaning and standardizing unemployment, interest rate, GDP, and exchange rate data
Reshaping datasets into a country‑year panel format
Merging all datasets into a unified panel
Exporting the final cleaned dataset used for all subsequent analysis

---

## 📦 Output dataset:
data/processed/final_panel_dataset.csv

2️⃣ Analysis and Regression Results
Path: notebooks/02_analysis_and_regression.ipynb
This notebook covers:

Exploratory data analysis and professional visualizations
Baseline pooled OLS regression
Fixed‑effects regression (country & year)
Lagged interest rate robustness tests
Crisis dummy models (2008 & 2020)
Crisis interaction model
Interpretation of results and final conclusions

## 📊 Input dataset:
data/processed/final_panel_dataset.csv

🧹 Data Preparation
The project integrates multiple macroeconomic datasets, including:

- Unemployment rates
- Real interest rates
- GDP
- Country‑level indicators

Because these datasets originate from different sources and formats, extensive preprocessing was required:

- Unemployment data were transformed from wide to long (country‑year) format
- Real interest rate data were standardized and cleaned
- GDP data were reshaped from wide to long format
- Cross‑sectional country datasets were merged appropriately

The final result is a clean, harmonized country‑year panel dataset suitable for econometric analysis.

---

## 🔍 Exploratory Analysis
Exploratory analysis reveals strong heterogeneity in unemployment outcomes across countries and over time. Key findings include:

- Persistent structural differences in unemployment levels across countries
- Smooth global averages masking substantial country‑specific variation
- Clear labor market disruptions during major global shocks

Five professional visualizations support these insights:

- Global unemployment and real interest rate trends
- Interest rate–unemployment scatter with regression line
- Country‑level unemployment trajectories
- GDP versus unemployment relationship
- Unemployment distributions across crisis periods

These plots motivate the use of fixed‑effects and crisis‑focused econometric models.

## Econometric Methodology
The empirical strategy follows a layered approach:
- Baseline Models

- Pooled OLS as a benchmark specification
Two‑way fixed effects regression controlling for country and year heterogeneity

- Robustness and Crisis Models

Lagged interest rate model to test delayed monetary transmission
Crisis dummy models isolating the 2008 and 2020 shocks
Crisis interaction model examining whether monetary transmission changes during crises

All regressions use cluster‑robust standard errors at the country level, consistent with best practices in applied panel data econometrics.

---

## 📈 Key Results

- **Real interest rates** do not exhibit a statistically significant direct or lagged effect on unemployment once country and year fixed effects are included.
- **GDP** is negatively associated with unemployment, though the effect is modest in magnitude.
- The **COVID‑19 pandemic (2020)** produced a strong and statistically significant increase in unemployment across countries.
- The **2008 Global Financial Crisis** shows weaker and more complex labor‑market effects.
- **Crisis interaction models** indicate that monetary policy effectiveness did not change significantly during the Global Financial Crisis.
- Persistent **country‑specific structural factors** dominate unemployment dynamics.

---

## ✅ Conclusions
- Overall, the findings indicate that global unemployment dynamics are driven primarily by structural country characteristics and major economic shocks, rather than by interest rate movements alone. While monetary policy remains an essential stabilization tool, its direct influence on unemployment appears indirect, heterogeneous, and context‑dependent in a global panel setting.
- The COVID‑19 pandemic stands out as a uniquely severe labor market shock, while the effects of the 2008 crisis appear to have propagated through more complex institutional and structural channels. These results highlight the importance of labor market resilience, institutional quality, and complementary fiscal and structural policies alongside monetary intervention.

---

## 🛠️ Tools and Libraries

- Python
- pandas
- numpy
- matplotlib
- seaborn
- statsmodels

---

## 👤 Author
AWAIS SHAKEEL PASHA
Macroeconomic & Data Analysis Project
Islamabad, Pakistan

---

## 📌 Notes
This repository is intended for:

Academic coursework
Applied econometrics practice
Portfolio demonstration
Interview and review discussions
