# 📊 Skill Gap Analysis & Career Path Optimization

> A data-driven exploration of the global tech job market — identifying the most in-demand skills, analyzing salary trends, forecasting future demand, and revealing actionable insights to bridge the gap between industry needs and workforce readiness.

---

## 👥 Team Members

* **Tirth Chankeshwara**
* **Tejas Deshmane**
* **Mahesh Bhimde**

---

## 🎯 Problem Statement

The rapid evolution of technology has created a significant **skill gap** between what industries demand and what professionals currently possess. This project aims to:

* Forecast **future demand** for tech skills (12–18 months ahead)
* Quantify **skill gaps** across roles, locations, and experience levels
* Analyze **salary variations** based on skill combinations
* Provide **data-driven career recommendations** and **learning paths**
* Visualize trends and insights through an **interactive dashboard**

---

## 🗂️ Data Sources

We integrated three primary Kaggle datasets:

1. **Data Science Job Market (brsahan)** – 10K+ listings; job titles, locations, salaries, and skills.
2. **Job-Skill-Set (batuhanmutlu)** – curated mapping of job roles to extracted skill sets.
3. **Global AI Job Market (bismasajjad)** – 15K+ listings across 50+ countries with salary, experience, and company data.

**Integration Strategy:** Columns were harmonized (job titles, skills, currencies, experience) and merged into a unified dataset `cleaned_master.csv`.

---

## ⚙️ Methodology Overview

### **Phase 1 – Data Collection & Cleaning**

* Gathered raw datasets from Kaggle sources.
* Standardized schema, handled missing values, duplicates, and outliers.
* Validated integrity using automated quality checks.
* Generated `data_quality_report.json` summarizing completeness and validity.

### **Phase 2 – Pre-processing & Feature Engineering**

* Standardized skills through normalization and taxonomy mapping.
* Engineered features: `salary_midpoint`, `skill_count`, `posting_year`, etc.
* Generated profiling snapshots (`profiling_categorical_snapshot.csv`, `profiling_numeric_snapshot.csv`).
* Exported unified cleaned dataset for downstream modeling.

### **Phase 3 – Exploratory Data Analysis**

* Conducted univariate, bivariate, and multivariate analysis on `cleaned_master.csv`.
* Identified correlations, hiring trends, salary distributions, and geographic demand.
* Generated 30+ visualizations stored in `/outputs/figures/`.
* Derived insights:

  * Salary increases significantly with seniority and full-time roles.
  * Remote jobs offer competitive compensation.
  * Most in-demand skills: **Python, SQL, Machine Learning, Cloud, Tableau.**
  * Leading hiring regions: **USA, India, UK, Germany.**

### **Phase 4 – Modeling & Evaluation (Completed)**

* **Forecasting:** Skill demand predictions (12–18 months) using **Naive, ARIMA, Prophet** models.
* **Salary Prediction:** Ridge, Random Forest, and XGBoost regressors achieving **R² > 0.7**.
* **Outputs:**

  * `models/salary_predictor.pkl`, `models/skill_demand_forecast.pkl`
  * `outputs/tables/model_metrics.csv`, `outputs/figures/model_performance.png`
* Insights:

  * AI/ML and Cloud-related skills expected to grow 15–20%.
  * Skills like **TensorFlow, PyTorch, and Kubernetes** offer the highest salary premiums.

### **Phase 5 – Visualization & Reporting (In Progress)**

* Building a Power BI dashboard integrating forecast and salary insights.
* Preparing final report and presentation for Datathon submission.

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
│   ├── external/                    # Supporting/reference datasets
│   ├── processed/                   # Cleaned and merged data
│   │   ├── cleaned_master.csv
│   │   ├── X_train.csv / y_train.csv
│   │   └── X_test.csv / y_test.csv
│   └── raw/                         # Original Kaggle datasets
│       ├── dataset1_data_science_job.csv
│       ├── dataset2_all_job_post.csv
│       ├── dataset3_ai_job_dataset.csv
│       └── dataset3_ai_job_dataset1.csv
│
├── models/                          # Trained model artifacts
│   ├── salary_predictor.pkl
│   ├── skill_demand_forecast.pkl
│   └── skill_clusterer.pkl
│
├── notebooks/                       # Jupyter notebooks by phase
│   ├── 04_feature_engineering.ipynb
│   ├── 05_modeling_forecasting.ipynb
│   ├── 06_modeling_salary_prediction.ipynb
│
├── outputs/
│   ├── figures/                     # Visualizations & charts
│   └── tables/                      # Aggregated model metrics
│
├── reports/                         # Reports & documentation
│   ├── model_evaluation_report.json
│   ├── model_validation_notes.md
│   └── data_quality_report.json
│
└── src/                             # Optional Python scripts for automation
```

---

## 🦎 Key Deliverables (Phase-Wise)

| Phase   | Deliverable                                        | Status         |
| ------- | -------------------------------------------------- | -------------- |
| Phase 1 | Data sourcing, schema validation                   | ✅ Completed    |
| Phase 2 | Data cleaning, feature engineering, quality report | ✅ Completed    |
| Phase 3 | Exploratory analysis & insights                    | ✅ Completed    |
| Phase 4 | Modeling, forecasting, salary prediction           | ✅ Completed    |
| Phase 5 | Dashboard, final report & presentation             | 🚧 In Progress |

---

## 📊 Current Outputs

* **Processed Data:** `cleaned_master.csv` (36 columns, ~36K rows)
* **Models:** `salary_predictor.pkl`, `skill_demand_forecast.pkl`
* **Reports:** `model_evaluation_report.json`, `data_quality_report.json`
* **Visuals:** `model_performance.png`, `feature_importance.png`, `forecast_trend.png`
* **Tables:** `model_metrics.csv`, `forecast_results.csv`, `feature_summary.csv`

---

## 🚀 How to Run

```bash
git clone https://github.com/<username>/datathon-2025.git
cd datathon-2025
pip install -r requirements.txt
jupyter notebook notebooks/06_modeling_salary_prediction.ipynb
```

---

## 📧 Contact

**Team Contact:** [work.tejasx@gmail.com](mailto:work.tejasx@gmail.com)

---

