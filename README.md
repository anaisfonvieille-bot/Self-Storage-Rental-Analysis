# 📦 Self-Storage Rental Analysis

![Python](https://img.shields.io/badge/Python-Data%20Analysis-3776AB?logo=python&logoColor=white)
![Power BI](https://img.shields.io/badge/Power%20BI-Dashboard-F2C811?logo=powerbi&logoColor=black)
![Machine Learning](https://img.shields.io/badge/Machine%20Learning-Predictive%20Models-2E8B57)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626?logo=jupyter&logoColor=white)
![Data](https://img.shields.io/badge/Data-Anonymized-0078D4)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen)

🌐 **Language:** English | [Français](README_FR.md)

## 📌 Project Overview

This project was developed for a self-storage company operating four storage centres.

The company had contract data distributed across several files, but no consolidated analytical solution and very limited customer-level information.

The objective was to transform the available contract data into useful business insights, build a Power BI monitoring dashboard, and explore predictive models capable of identifying contracts with a higher risk of early termination or cancellation.

> The models support prioritisation and decision-making. They do not replace human analysis.
## 🎯 Business Problem

The company wanted to:

- Centralise and clean contract data from several sources.
- Monitor activity through Power BI, which was not previously developed.
- Identify the types of contracts most likely to end after 4, 6 or 12 months.
- Analyse contractual profiles most associated with cancellations before the contract start date.
- Prioritise commercial and retention actions.
- Define which additional customer data should be collected in the future.

## ✅ Project Objectives

| Objective | Business value |
|---|---|
| Consolidate the available files | Create one reliable analytical dataset |
| Improve data quality | Produce consistent and reusable indicators |
| Build a Power BI dashboard | Make operational monitoring easier |
| Predict early contract departures | Identify contracts requiring attention |
| Analyse cancellations | Better understand recurring contractual profiles |
| Recommend future data collection | Improve future analyses and predictive models |
## 🗂️ Data Scope

The analysis is based on anonymised contractual and operational data from four self-storage centres.

The original data were supplied in eight files and consolidated into a single analytical dataset. Public deliverables exclude raw company data, employee names, real centre names and contract identifiers.

### Available information

- Contract status and dates
- Storage characteristics
- Payment mode and recurring period
- Financial and tax-related contract fields
- Discounts and contractual variables
- Anonymised centre information

### Current limitations

The company does not yet collect enough customer-profile information. Variables such as age group, occupation, acquisition channel, storage motive, satisfaction, cancellation reason or departure reason were unavailable.

Consequently:

- The models rely mainly on contractual characteristics.
- Observed relationships must not be interpreted as causality.
- Predictive results are intended for prioritisation, not automatic decisions.
- Occupancy, margin, net profitability and actual relocation delays were outside the available scope.
## 🛠️ Technologies

- **Python** — data preparation, quality controls and modelling
- **Pandas / NumPy** — data manipulation
- **Matplotlib / Seaborn** — exploratory visualisation
- **Scikit-learn** — predictive modelling and evaluation
- **Jupyter Notebook** — reproducible analytical workflow
- **Power BI** — operational and management dashboard
- **Canva** — business presentation and recommendations

## 🔄 Methodology

1. Consolidation of eight source files
2. Structural and data-quality controls
3. Treatment of duplicates, missing values, dates, amounts and percentages
4. Exploratory analysis of contracts and cancellations
5. Construction of prediction targets for departures at 4, 6 and 12 months
6. Prevention of data leakage
7. Comparison of logistic regression, decision tree and random forest models
8. Evaluation using ROC-AUC, F1-score, precision, recall and confusion matrices
9. Interpretation using permutation importance and observed subgroup rates
10. Translation of results into practical business recommendations
## 🤖 Predictive Analysis

Two complementary predictive analyses were conducted.

### Early contract departure

The models estimate which contracts present characteristics associated with departure within:

- 4 months
- 6 months
- 12 months

Logistic regression, decision tree and random forest models were compared. Their performance was assessed using several complementary metrics rather than accuracy alone.

### Cancellation before contract start

A separate model analyses contractual profiles associated with cancellations before the planned start date.

Its predictive performance is considered moderate. It should therefore be used as a prioritisation aid and not as an automated decision tool.

## 📊 Power BI Dashboard

The anonymised Power BI report provides a consolidated view of business activity, including:

- Contract portfolio monitoring
- Active-contract revenue indicators
- Payment and cancellation monitoring
- Contract duration and departure analysis
- Comparisons between anonymised centres
- Filters supporting operational exploration

The public repository contains only an anonymised PDF export. The original Power BI file and company data are not published.
## 💡 Business Recommendations

- Contact higher-risk contracts proactively.
- Monitor short-duration and cancellation-prone contractual profiles.
- Review the role and profitability of discounts.
- Introduce alerts for contracts requiring commercial follow-up.
- Retrain and monitor predictive models as new data become available.
- Collect a small number of relevant customer variables through short dropdown lists.
- Record cancellation and departure reasons consistently.
- Keep human validation at the centre of every commercial decision.

## 📚 Project Deliverables

### 📓 Jupyter Notebook

The notebook documents:

- Data consolidation and cleaning
- Data-quality controls
- Exploratory analysis
- Feature preparation
- Predictive modelling
- Model evaluation and interpretation

### 📊 Power BI Report

The anonymised report presents the main operational and analytical indicators through a clear management dashboard.

### 🎨 Canva Presentation

The presentation explains the business problem, methodology, results, limitations and recommendations in a business-oriented format.

## 📁 Repository Structure

```text
Self-Storage-Rental-Analysis/
├── README.md
├── requirements.txt
├── .gitignore
├── notebooks/
│   └── self_storage_analysis.ipynb
├── powerbi/
│   └── powerbi_dashboard_anonymized.pdf
├── presentation/
│   └── self_storage_analysis_report.pdf
└── images/
    └── dashboard_overview.png
```

## 🔐 Confidentiality

This repository is designed for portfolio publication.

It does **not** include:

- Raw CSV or Excel company data
- Real centre names
- Employee names
- Contract identifiers
- The original Power BI file
- Confidential operational exports

All published documents have been checked and anonymised before publication.

## ⚠️ Responsible Use

The predictive models identify statistical patterns in the available contract data. They must not be used to make fully automated commercial decisions.

Predictions should always be reviewed by a human and combined with operational knowledge.

## 👩‍💻 Author

**Anaïs Fonvieille**

Data analysis, dashboard design and predictive modelling project.
