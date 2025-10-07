# 📊 Skill Gap Analysis & Career Path Optimization

> A data-driven exploration of the global tech job market — identifying the most in-demand skills, analyzing salary trends, and revealing actionable insights to bridge the gap between industry demand and workforce readiness.


**📅 Academic Year:** 2025–26 (Semester VII Datathon)

---

## 👥 Team Members

* **Tirth Chankeshwara**
* **Tejas Deshmane**
* **Mahesh Bhimde**

---

## 🎯 Problem Statement

The rapid evolution of technology has created a significant **skill gap** between what industries demand and what professionals currently possess. This project aims to:

* Forecast the **future demand** of tech skills (12–18 months ahead)
* Quantify **skill gaps** across roles, locations, and experience levels
* Analyze **salary variations** based on skill combinations
* Provide **data-driven career recommendations** and **learning paths**
* Visualize skill trends and insights through an **interactive dashboard**

---

## 📂 Data Sources

We integrated three primary Kaggle datasets:

1. **Data Science Job Market (brsahan)** – 10K+ listings; job titles, locations, salaries, skills.
2. **Job-Skill-Set (batuhanmutlu)** – curated mapping of job roles to extracted skill sets.
3. **Global AI Job Market (bismasajjad)** – 15K+ listings across 50+ countries with salary, experience, and company data.

**Integration Strategy:** Columns were harmonized (job titles, skills, currencies, experience) and merged into a unified `cleaned_master.csv` dataset.

---

## ⚙️ Methodology Overview

### **Phase 1 – Data Collection & Cleaning**

* Gathered raw datasets from Kaggle sources.
* Standardized column names and data types.
* Handled missing values, duplicates, and outliers.
* Generated `data_quality_report.json` for validation metrics.

### **Phase 2 – Pre-processing & Feature Engineering**

* Standardized skills using text normalization and taxonomy mapping.
* Engineered new features: `salary_midpoint`, `skill_count`, `posting_year`, etc.
* Created profiling snapshots (categorical & numerical).
* Exported cleaned dataset (`cleaned_master.csv`) for downstream analysis.

### **Phase 3 – Exploratory Data Analysis (Ongoing)**

* Perform univariate, bivariate, and multivariate analyses.
* Identify correlations, skill trends, and salary distributions.
* Generate key insights for model design (forecasting, prediction, clustering).

### **Phase 4 – Modeling & Forecasting**

* Apply ML algorithms: ARIMA/Prophet (skill forecasting), XGBoost (salary prediction), clustering for role patterns.

### **Phase 5 – Visualization & Reporting**

* Develop Power BI dashboard showing trends, forecasts, and insights.
* Submit final report and presentation as per Datathon guidelines.

---

## 📁 Repository Structure

```
datathon-2025/
│
├── .gitignore
├── LICENSE
├── README.md
├── requirements.txt
│
├── dashboards/                      # Power BI / Tableau dashboards
│
├── data/
│   ├── README.md                    # Data dictionary and sources
│   ├── external/                    # Supporting or reference datasets
│   ├── processed/                   # Cleaned and merged data
│   │   └── cleaned_master.csv
│   └── raw/                         # Original Kaggle datasets
│       ├── dataset1_data_science_job.csv
│       ├── dataset2_all_job_post.csv
│       ├── dataset3_ai_job_dataset.csv
│       └── dataset3_ai_job_dataset1.csv
│
├── models/                          # Trained model files (.pkl, .sav)
│
├── notebooks/                       # Jupyter notebooks for each phase
│   ├── 01_data_collection.ipynb
│   └── 02_data_cleaning.ipynb
│
├── outputs/
│   ├── figures/                     # Visuals from EDA and reports
│   ├── insights/                    # Textual insight summaries
│   └── tables/                      # Aggregated metrics / CSV summaries
│
├── reports/                         # Reports and data profiling results
│   ├── data_quality_report.json
│   ├── profiling_categorical_snapshot.csv
│   └── profiling_numeric_snapshot.csv
│
└── src/                             # Python scripts for preprocessing & modeling
```

---

## 🧮 Key Deliverables (Phase-Wise)

| Phase   | Deliverable                                        | Status         |
| ------- | -------------------------------------------------- | -------------- |
| Phase 1 | Dataset sourcing, schema validation                | ✅ Completed    |
| Phase 2 | Data cleaning, feature engineering, quality report | ✅ Completed    |
| Phase 3 | Exploratory Data Analysis & insight generation     | 🔄 In Progress |
| Phase 4 | Modeling & evaluation                              | ⏳ Upcoming     |
| Phase 5 | Dashboard, final report & presentation             | ⏳ Upcoming     |

---

## 📊 Current Outputs

* `cleaned_master.csv` → Unified master dataset (36 columns, ~36K rows)
* `profiling_categorical_snapshot.csv` / `profiling_numeric_snapshot.csv` → Profiling statistics
* `data_quality_report.json` → Completeness & validity summary

---

## 🚀 How to Run

```bash
git clone https://github.com/<username>/datathon-2025.git
cd datathon-2025
pip install -r requirements.txt
jupyter notebook notebooks/02_data_cleaning.ipynb
```

---

## 🎓 Academic Context

This project is developed as part of the **Data Analytics ISE Datathon (Sem VII)** under the Department of Electronics Engineering, WIT Solapur. It demonstrates application of the full **OSEMN pipeline** — *Obtain, Scrub, Explore, Model, iNterpret*.

---

## 📧 Contact

**Team Contact:** [work.tejasx@gmail.com](mailto:work.tejasx@gmail.com)

---

📘 *Walchand Institute of Technology, Solapur – Data Analytics Datathon 2025–26*
