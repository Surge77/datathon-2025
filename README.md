# 📊 Skill Gap Analysis & Career Path Optimization

> Analyzing the tech job market to help you make smarter career decisions and predict what skills will be in demand next.

**🏫 Institution:** Walchand Institute of Technology, Solapur  
**📅 Academic Year:** 2025-26 (Semester VII Datathon)

---

## 👥 Team

- Tirth Chankeshwara
- Tejas Deshmane  
- Mahesh Bhimde

---

## 🎯 What We're Solving

There's a huge gap between what tech professionals know and what companies actually need. We're tackling this by:

- 📈 Predicting which skills will be hot in the next 12–18 months
- 🔍 Finding the exact gaps between what people know vs. what jobs require
- 💰 Showing how different skill combinations affect your salary
- 🗺️ Recommending the best learning paths for career growth
- 🌍 Mapping which skills are in demand in different locations

---

## 📦 Our Data Sources

We're working with three Kaggle datasets:

1. **Data Science Job Market Dataset** — 10,000+ real job listings with skills, salaries, and locations
2. **Job-Skill-Set Dataset** — Already processed skill data mapped to specific jobs
3. **Global AI Job Market & Salary Trends 2025** — 15,000+ listings from 50+ countries worldwide

We're combining these by standardizing skill names and merging based on common fields like skills, job titles, and salaries.

---

## 🛠️ How We're Doing It

### **Phase 1: Cleaning the Data**
First, we need clean data. This means fixing missing values, removing duplicates, handling weird outliers, and creating new useful features like skill scores and normalized salaries.

### **Phase 2: Understanding the Data**
Here we dig deep into what the data tells us. Which skills appear most? How do salaries vary? What's trending from 2022 to 2025? Where are jobs located? We use heatmaps, graphs, and charts to visualize everything.

### **Phase 3: Building Prediction Models**
This is where machine learning comes in:
- **Forecasting skill demand** using Prophet and ARIMA
- **Predicting salaries** with Random Forest and XGBoost
- **Grouping similar careers** using clustering
- **Classifying job roles** automatically

### **Phase 4: Creating the Dashboard**
We're building an interactive dashboard where you can:
- Track which skills are trending
- Estimate your potential salary
- Explore career paths
- See skill demand by location

---

## 📁 What You'll Find Here

```
├── data/                    # Info about our datasets
├── notebooks/               # Our analysis step-by-step
│   ├── 01_preprocessing.ipynb
│   ├── 02_eda.ipynb
│   └── 03_modeling.ipynb
├── scripts/                 # Python code we wrote
├── outputs/                 # All our graphs and charts
├── dashboards/              # Interactive dashboards
├── report/                  # Final writeup and presentation
└── requirements.txt         # Libraries you'll need
```

---

## 🚀 Want to Run This Yourself?

**1. Get the code:**
```bash
git clone https://github.com/<username>/datathon-2025-skill-gap.git
cd datathon-2025-skill-gap
```

**2. Install what you need:**
```bash
pip install -r requirements.txt
```

**3. Run the notebooks:**
Just open them in order (preprocessing → EDA → modeling) and run all cells.

**4. Check out the dashboard:**
Open the Power BI or Tableau files in the `dashboards/` folder.

---

## 📅 Our Timeline

| Phase | Date | What We're Delivering |
|-------|------|----------------------|
| Phase 1 | Sep 6, 2025 | Cleaned and ready data |
| Phase 2 | Sep 13, 2025 | All our analysis and insights |
| Phase 3 | Sep 27, 2025 | Working prediction models |
| Phase 4 | Oct 8, 2025 | Dashboard + final report |

---

## 🎯 What Success Looks Like

- ✅ **Accurate predictions** — At least 85% accuracy on our forecasts
- ✅ **Useful insights** — Recommendations you can actually act on
- ✅ **Easy-to-use dashboard** — Anyone should be able to explore the data
- ✅ **Clear documentation** — Everything explained so you can reproduce our work

---

## 📧 Questions?

Reach out to us: [work.tejasx@gmail.com](mailto:work.tejasx@gmail.com)

---

⚡ *Datathon Project - Semester VII | Walchand Institute of Technology, Solapur*