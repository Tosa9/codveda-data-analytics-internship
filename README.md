# 📊 Codveda Technologies — Data Analytics Internship

<div align="center">

![Python](https://img.shields.io/badge/Python-3.10+-blue?style=for-the-badge&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-2.2+-green?style=for-the-badge&logo=pandas&logoColor=white)
![Scikit-Learn](https://img.shields.io/badge/ScikitLearn-1.4+-orange?style=for-the-badge&logo=scikit-learn&logoColor=white)
![Power BI](https://img.shields.io/badge/Power%20BI-Dashboard-yellow?style=for-the-badge&logo=powerbi&logoColor=white)
![Tableau](https://img.shields.io/badge/Tableau-Public-blue?style=for-the-badge&logo=tableau&logoColor=white)

**Intern:** Omokhoa Oshose Tosayoname &nbsp;|&nbsp; **ID:** CV/A1/61250 &nbsp;|&nbsp; **Role:** Data Analysis Intern

**Organisation:** Codveda Technologies &nbsp;|&nbsp; **Duration:** March – May 2026 &nbsp;|&nbsp; **Mode:** Remote

</div>

---

## 📋 Table of Contents

1. [Project Overview](#-project-overview)
2. [Repository Structure](#-repository-structure)
3. [Tools and Technologies](#-tools-and-technologies)
4. [Level 1 — Basic Data Analysis](#-level-1--basic-data-analysis)
5. [Level 2 — Intermediate Data Analysis](#-level-2--intermediate-data-analysis)
6. [Level 3 — Advanced Data Analysis](#-level-3--advanced-data-analysis)
7. [Key Findings Summary](#-key-findings-summary)
8. [Dashboards](#-dashboards)
9. [How to Run the Notebooks](#-how-to-run-the-notebooks)
10. [Connect With Me](#-connect-with-me)

---

## 🎯 Project Overview

This repository contains all completed work for the **Codveda Technologies Data Analytics Internship** — a hands-on, project-based programme designed to develop real-world data analytics skills across three progressive levels.

Over the course of the internship, six data analytics tasks were completed spanning the full analytics pipeline:

| Level | Focus | Tasks Completed |
|---|---|---|
| **Level 1 — Basic** | Data exploration and visualisation | EDA · Basic Data Visualisation |
| **Level 2 — Intermediate** | Pattern discovery and time-based analysis | Time Series Analysis · K-Means Clustering |
| **Level 3 — Advanced** | NLP and business intelligence | Sentiment Analysis · Interactive Dashboards |

All tasks are documented in fully executable **Jupyter Notebooks** with step-by-step explanations, inline visualisations, and analytical insights. Dashboards were built in both **Power BI** and **Tableau Public**.

---

## 📁 Repository Structure

```
codveda-data-analytics-internship/
│
├── README.md
├── requirements.txt
│
├── Level_1_Basic/
│   ├── Level_1_Basic_Data_Analysis.ipynb
│   └── outputs/
│       ├── 01_histograms.png
│       ├── 02_boxplots.png
│       ├── 03_scatter_plots.png
│       ├── 04_correlation_heatmap.png
│       ├── 05_bar_plot.png
│       └── 06_line_charts.png
│
├── Level_2_Intermediate/
│   ├── Level_2_Intermediate_Data_Analysis.ipynb
│   └── outputs/
│       ├── 07_aapl_raw_timeseries.png
│       ├── 08_moving_averages.png
│       ├── 09_decomposition.png
│       ├── 10_multi_stock_comparison.png
│       ├── 11_elbow_method.png
│       └── 12_kmeans_clusters.png
│
├── Level_3_Advanced/
│   ├── Level_3_Advanced_Data_Analysis.ipynb
│   └── outputs/
│       ├── 13_sentiment_distribution.png
│       ├── 14_polarity_subjectivity.png
│       ├── 15_sentiment_by_platform_country.png
│       ├── 16_sentiment_over_time.png
│       ├── 17_word_clouds.png
│       ├── 18_top_words.png
│       ├── 19_polarity_boxplot.png
│       ├── powerbi_dashboard_screenshot.png
│       └── tableau_dashboard_screenshot.png
│
└── datasets/
    ├── iris.csv
    ├── Stock_Prices_Data_Set.csv
    ├── Sentiment_dataset.csv
    ├── Churn_Dashboard_Data.csv
    ├── churn-bigml-80.csv
    └── churn-bigml-20.csv
```

---

## 🛠 Tools and Technologies

| Category | Tools |
|---|---|
| **Language** | Python 3.10+ |
| **Data Manipulation** | pandas, numpy |
| **Visualisation** | matplotlib, seaborn, WordCloud |
| **Machine Learning** | scikit-learn (KMeans, StandardScaler, PCA) |
| **Time Series** | statsmodels |
| **NLP** | TextBlob, re (regex) |
| **Business Intelligence** | Microsoft Power BI Desktop, Tableau Public |
| **Development Environment** | Jupyter Notebook, Google Colab |
| **Version Control** | Git, GitHub |

---

## 📗 Level 1 — Basic Data Analysis

**Dataset:** Iris Dataset (150 records, 5 features)
**Notebook:** [`Level_1_Basic_Data_Analysis.ipynb`](Level_1_Basic/Level_1_Basic_Data_Analysis.ipynb)

### Task 2 — Exploratory Data Analysis (EDA)

Performed a comprehensive exploratory analysis of the Iris dataset to understand its structure, distribution, and feature relationships.

**Steps taken:**
- Removed 3 duplicate rows identified during initial inspection
- Calculated mean, median, mode, and standard deviation for all four numerical features
- Computed a full correlation matrix and interpreted pairwise relationships
- Generated per-species summary statistics revealing how the three flower species differ

**Key findings:**

| Finding | Detail |
|---|---|
| Most variable feature | Petal length (std = 1.76 cm) |
| Most consistent feature | Sepal width (std = 0.44 cm) |
| Strongest correlation | Petal length vs Petal width (r = 0.96) |
| Most separable species | *Iris setosa* — distinctly small petals |

### Task 3 — Basic Data Visualisation

Created six publication-quality charts to communicate the dataset's structure and relationships:

| Chart | Insight |
|---|---|
| Histograms | Setosa petal measurements cluster far below other species |
| Boxplots | Virginica has widest spread; setosa most consistent |
| Scatter plots | Petal dimensions form near-perfect linear clusters by species |
| Correlation heatmap | Petal features almost perfectly correlated (r = 0.96) |
| Bar plot | Virginica largest across all features |
| Line charts | Petal bands clearly species-separated across all samples |

---

## 📘 Level 2 — Intermediate Data Analysis

**Datasets:** Stock Prices Dataset (497,472 rows, 505 symbols) · Iris Dataset
**Notebook:** [`Level_2_Intermediate_Data_Analysis.ipynb`](Level_2_Intermediate/Level_2_Intermediate_Data_Analysis.ipynb)

### Task 2 — Time Series Analysis

Analysed Apple Inc. (AAPL) daily closing prices from January 2014 to December 2017.

**Steps taken:**
- Filtered AAPL from 505 stock symbols
- Converted date strings to datetime and set as index
- Computed 30-day and 90-day moving averages
- Applied multiplicative seasonal decomposition (period = 252 trading days)
- Normalised and compared AAPL against MSFT, GOOGL, and AMZN

**Key findings:**

| Finding | Detail |
|---|---|
| Total price return | +114.2% ($79.02 → $169.23) |
| Price minimum | $71.40 (mid-2016) |
| Price maximum | $176.42 (late 2017) |
| Best performing peer | Amazon (AMZN) — ~4× return over same period |
| Decomposition model | Multiplicative (annual seasonal cycle detected) |

### Task 3 — Clustering Analysis (K-Means)

Applied unsupervised machine learning to the Iris dataset to discover natural groupings without using species labels.

**Steps taken:**
- Standardised all four features using StandardScaler (z = (x − μ) / σ)
- Applied the Elbow Method across K = 1 to 10 — optimal K = 3 confirmed
- Fitted K-Means with K=3 and validated against true species labels
- Visualised clusters using PCA projection (97.7% variance explained)

**Key findings:**

| Finding | Detail |
|---|---|
| Optimal clusters | K = 3 (confirmed by elbow method) |
| Setosa accuracy | 100% — all 48 records correctly isolated |
| Overall accuracy | ~85% — overlap between versicolor/virginica |
| PCA variance explained | 97.7% across two components |

---

## 📙 Level 3 — Advanced Data Analysis

**Datasets:** Social Media Sentiment Dataset (732 posts) · Customer Churn Dataset (3,333 customers)
**Notebook:** [`Level_3_Advanced_Data_Analysis.ipynb`](Level_3_Advanced/Level_3_Advanced_Data_Analysis.ipynb)

### Task 3 — NLP Sentiment Analysis

Built a complete text analytics pipeline to classify social media posts as Positive, Negative, or Neutral.

**Pipeline stages:**
1. Data cleaning — stripped whitespace, dropped redundant columns
2. Emotion label mapping — consolidated 279 unique labels into 3 classes
3. Text preprocessing — lowercase, URL/mention removal, tokenisation, stopword removal, lemmatisation
4. TextBlob sentiment scoring — polarity and subjectivity computed for all 732 posts
5. Visualisation — 7 charts including word clouds, frequency analysis, and platform breakdowns

**Key findings:**

| Finding | Detail |
|---|---|
| Sentiment distribution | 64.6% Positive · 28.3% Negative · 7.1% Neutral |
| TextBlob agreement rate | 46.2% — expected given nuanced emotion labels |
| Mean polarity — Positive | +0.191 |
| Mean polarity — Negative | −0.106 |
| Top positive words | beautiful, enjoy, feel, amazing, love |
| Top negative words | fearful, shadows, storm, heartbreak, lost |

### Task 2 — Interactive Dashboard (Power BI + Tableau)

Built a Customer Churn Analysis Dashboard in both Power BI and Tableau Public using a combined churn dataset of 3,333 customer records with 7 engineered features.

**Dashboard visuals:**
- KPI Cards (Total Customers · Churn Rate · Avg Charge · Avg Service Calls)
- Churn by International Plan (100% Stacked Bar)
- Churn by Service Call Risk (Stacked Column — staircase pattern)
- Total Charge Distribution (Histogram)
- Churn Rate by State (Filled Map)
- Churned Customers by Tenure Band (Pie/Donut Chart)
- Day Usage vs Charge (Scatter Plot)
- Interactive Filters (International Plan · Voice Mail Plan)

**Key findings:**

| Finding | Detail |
|---|---|
| Overall churn rate | 14.5% (483 of 3,333 customers) |
| Highest churn driver | International plan (~4× higher churn rate) |
| Critical risk threshold | 5+ customer service calls |
| Highest-risk tenure segment | Established (100-149 days) — 41.4% of churned |

---

## 💡 Key Findings Summary

Across all six tasks, three cross-cutting analytical themes emerged:

**1. Feature importance is not obvious from inspection alone**
In the Iris dataset, petal dimensions proved far more discriminating than sepal dimensions — something that only became apparent through EDA and confirmed by K-Means clustering. Similarly in the churn dataset, the international plan variable was not the most prominent field but turned out to be the strongest churn predictor.

**2. Real-world data is always messy**
The sentiment dataset arrived with 279 unique emotion labels, whitespace inconsistencies, and redundant index columns. The churn dataset required feature engineering before it could support meaningful dashboard analysis. Professional data work begins with cleaning, not analysis.

**3. Communication is as important as computation**
The same churn insights that exist as numbers in a Python script become genuinely actionable when presented in an interactive Power BI or Tableau dashboard that a business stakeholder can explore without technical knowledge.

---

## 📊 Dashboards

### Tableau Public Dashboard (Live & Interactive)
🔗 **[Customer Churn Analysis Dashboard](https://public.tableau.com/views/Book1_17747150703190/Dashboard1)**

> Click the link above to explore the fully interactive dashboard — filter by International Plan, Voice Mail Plan, and click any chart to cross-filter the entire dashboard.

### Power BI Dashboard
Built in Microsoft Power BI Desktop. Screenshot available in [`Level_3_Advanced/outputs/powerbi_dashboard_screenshot.png`](Level_3_Advanced/outputs/powerbi_dashboard_screenshot.png)

---

## ▶ How to Run the Notebooks

### Option 1 — Google Colab (Recommended, no setup required)

1. Open the notebook directly in Google Colab
2. Upload the required datasets to a `datasets/` folder in the Colab file system
3. Run all cells top to bottom — all dependencies are installed automatically

### Option 2 — Local Jupyter Notebook

**Prerequisites:** Python 3.10+, pip

**Step 1 — Clone the repository:**
```bash
git clone https://github.com/Tosa9/codveda-data-analytics-internship.git
cd codveda-data-analytics-internship
```

**Step 2 — Install dependencies:**
```bash
pip install -r requirements.txt
```

**Step 3 — Launch Jupyter:**
```bash
jupyter notebook
```

**Step 4 — Open any notebook** from the Level folders and run all cells.

### Dataset Note
Datasets are included in the `datasets/` folder. The Stock Prices dataset (~24MB) may take a moment to load.

---

## 📦 Requirements

```
pandas>=2.0
numpy>=1.24
matplotlib>=3.7
seaborn>=0.12
scikit-learn>=1.3
statsmodels>=0.14
textblob>=0.17
wordcloud>=1.9
jupyter>=1.0
nbformat>=5.9
```

Install all dependencies with:
```bash
pip install -r requirements.txt
```

---

## 🤝 Connect With Me

**Omokhoa Oshose Tosayoname**
Data Science/Analysis Intern | Mechanical Engineering Student | Junior Project Manager

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue?style=flat&logo=linkedin)](https://www.linkedin.com/in/oshose-omokhoa-3982aa364/)
[![GitHub](https://img.shields.io/badge/GitHub-Follow-black?style=flat&logo=github)](https://github.com/Tosa9)
[![X](https://img.shields.io/badge/X-Follow-black?style=flat&logo=x)](https://x.com/Tosa_omokhoa)

---

<div align="center">

*Completed as part of the Codveda Technologies Data Analytics Internship Programme*
*Intern ID: CV/A1/61250 | March – May 2026*

**#Codveda #CodvedaTech #CodvedaInternship #DataAnalytics #Python #MachineLearning**

</div>

