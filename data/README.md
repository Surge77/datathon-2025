# 🗂️ Data Folder Overview

This directory contains all datasets and derived artifacts used in the **Skill Gap Analysis & Career Path Optimization** Datathon project (Academic Year 2025–26, Semester VII).

Each subfolder represents a distinct stage of the data lifecycle — from raw collection to cleaned, processed, and analyzed forms.

---

## 📁 Folder Structure

| Folder       | Description                                                                                   |
| ------------ | --------------------------------------------------------------------------------------------- |
| `raw/`       | Original datasets downloaded from Kaggle and other public sources. Untouched and immutable.   |
| `processed/` | Cleaned, standardized, and merged datasets ready for analysis and modeling.                   |
| `reports/`   | Statistical profiling reports and data-quality metrics generated during cleaning.             |
| `external/`  | (Optional) Supporting reference datasets such as ESCO skill taxonomy or Glassdoor benchmarks. |

---

## 📄 Key Files

| File                                               | Stage     | Description                                                                                        |
| -------------------------------------------------- | --------- | -------------------------------------------------------------------------------------------------- |
| `dataset1_data_science_job.csv`                    | Raw       | Kaggle dataset containing data science and analytics job postings.                                 |
| `dataset2_all_job_post.csv`                        | Raw       | Dataset covering general job postings across multiple domains.                                     |
| `dataset3_ai_job_dataset.csv`                      | Raw       | AI-specific job postings dataset used for skill frequency comparison.                              |
| `dataset3_ai_job_dataset1.csv`                     | Raw       | Supplementary AI dataset variant for cross-validation.                                             |
| `cleaned_dataset1.csv`                             | Processed | Individually cleaned and standardized version of dataset1.                                         |
| `cleaned_dataset2.csv`                             | Processed | Individually cleaned and standardized version of dataset2.                                         |
| `cleaned_dataset3.csv`                             | Processed | Individually cleaned and standardized version of dataset3.                                         |
| `cleaned_master.csv` / `merged_master_dataset.csv` | Processed | Final unified dataset combining all sources (36,167 rows × 29 columns). Used for EDA and modeling. |
| `data_quality_report.json`                         | Reports   | Machine-readable summary of completeness, validity, and duplicates.                                |
| `profiling_categorical.csv`                        | Reports   | Summary of categorical column statistics (unique counts, top values, missing%).                    |
| `profiling_numerical.csv`                          | Reports   | Summary of numerical column statistics (mean, std, skewness, outlier ratio).                       |
| `anomalies.csv`                                    | Reports   | (Optional) Rows flagged during validation or de-duplication checks.                                |

---

## 🧾 Canonical Schema (Processed Dataset)

| Column Name            | Type   | Description                                                    |
| ---------------------- | ------ | -------------------------------------------------------------- |
| `job_id`               | string | Unique identifier for each job posting (generated if missing). |
| `job_title`            | string | Job title or designation.                                      |
| `job_category`         | string | Standardized category (e.g., Data Science, ML/AI, Analytics).  |
| `salary_in_usd`        | float  | Salary normalized to USD.                                      |
| `salary_currency`      | string | Original salary currency.                                      |
| `employee_residence`   | string | Country of residence of the employee.                          |
| `experience_level`     | string | EN (Entry), MI (Mid), SE (Senior), EX (Executive).             |
| `employment_type`      | string | FT (Full-Time), PT (Part-Time), CT (Contract), FL (Freelance). |
| `company_size`         | string | Company scale: S, M, or L.                                     |
| `company_location`     | string | Country or region of the company.                              |
| `required_skills`      | string | Comma-separated list of normalized skills.                     |
| `remote_ratio`         | int    | 0 = On-site, 50 = Hybrid, 100 = Fully Remote.                  |
| `posting_date`         | date   | Date when the job was posted.                                  |
| `application_deadline` | date   | Deadline for applying to the job.                              |
| `industry`             | string | Industry or domain category.                                   |
| `years_experience`     | int    | Required years of experience.                                  |
| `education_required`   | string | Minimum education level (if available).                        |
| `job_description`      | string | Text description of the job (optional).                        |
| `job_skill_set`        | string | Skill keywords extracted or parsed from job description.       |
| `__source__`           | string | Origin dataset identifier (dataset1, dataset2, etc.).          |

---

## ✅ Data Quality Summary

* **Rows:** 36,167
* **Columns:** 29
* **Duplicate Rows:** 0
* **Median Completeness:** ≈ 0.93
* **Posting Date Range:** 2010–2025 ✅
* **Remote Ratio Range:** 0–100 ✅
* **Salary Fields:** Non-negative and consistent ✅

---

## 🧩 Data Provenance & Licensing

All datasets were sourced from **public Kaggle repositories** and other open data portals under educational/research-use terms. No personally identifiable information (PII) is present.

**Do not redistribute** raw datasets publicly. Processed files are intended for academic evaluation only.

*Last updated: October 2025*
