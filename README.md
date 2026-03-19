# 🏃 Physical Activity & Sedentary Behavior Dashboard

> **SI Analytics 7-Day Data Visualization Challenge — Day 1**
> Built by [Olutayo Daniel Asaolu](https://www.linkedin.com/in/tayoasaolu)

![Dashboard Preview](physical_activity_dashboard.png)

---

## 📌 Overview

This project analyzes **daily physical activity and sedentary behavior patterns**
from adults and children, exploring how movement, BMI, and WHO activity targets
connect across age groups and gender.

### Core Question
> *"How do daily activity patterns differ by age group, sex, and BMI —
> and who meets WHO physical activity targets?"*

---

## 🔑 Key Insights

| # | Insight | Detail |
|---|---------|--------|
| 1 | **WHO Adherence Gap** | Only ~35% of participants meet WHO physical activity recommendations |
| 2 | **Gender MVPA Difference** | Males show significantly higher moderate-to-vigorous activity levels |
| 3 | **BMI-Activity Correlation** | Negative correlation between BMI and MVPA — more active = healthier BMI |
| 4 | **Sedentary Alarm** | Participants spend 8+ hours/day sedentary on average |
| 5 | **ML Segmentation** | K-Means clustering identifies 3 distinct health-behavior risk profiles |

---

## 🛠️ Technical Stack

| Category | Tools |
|----------|-------|
| **Language** | Python 3.10+ |
| **Data Manipulation** | pandas, NumPy |
| **Visualization** | matplotlib, seaborn |
| **Statistical Analysis** | scipy (t-tests, correlation, hypothesis testing) |
| **Machine Learning** | scikit-learn (K-Means clustering, StandardScaler) |
| **Version Control** | Git, GitHub |

---

## 📊 Dashboard Components

1. **KPI Cards** — Total participants, avg BMI, sedentary hours, MVPA, WHO compliance %
2. **Bar Chart** — Average MVPA (min/day) by age group and sex
3. **Stacked Bar** — WHO recommendation adherence by age group
4. **Grouped Column** — Sedentary vs. light activity comparison
5. **Scatter Plot** — BMI vs. MVPA colored by WHO compliance with trend line
6. **Box Plot** — MVPA distribution by sex with mean markers
7. **Violin Plot** — BMI distribution by age group
8. **Horizontal Stacked Bar** — Daily activity composition breakdown
9. **Donut Chart** — Overall WHO target compliance

### ML Extension
- **K-Means Clustering** segments participants into 3 health-behavior profiles:
  - Cluster 0: Active & Healthy
  - Cluster 1: Moderate Activity
  - Cluster 2: Sedentary & At Risk

![Clustering](clustering_health_risk.png)

---

## ☁️ Cloud & Production Architecture

This analysis framework can be scaled and productionized using:
┌──────────────┐ ┌──────────────┐ ┌──────────────┐
│ Data Source │───▶│ Azure Data │───▶│ Azure ML / │
│ (Wearables, │ │ Factory / │ │ SageMaker │
│ Surveys) │ │ AWS Glue │ │ (ML Models) │
└──────────────┘ └──────────────┘ └──────────────┘
│ │
▼ ▼
┌──────────────┐ ┌──────────────┐
│ BigQuery / │ │ Power BI / │
│ Azure SQL │ │ Tableau │
│ (Data Lake) │ │ (Dashboards) │
└──────────────┘ └──────────────┘


**Specific cloud applications:**
- **Azure ML / AWS SageMaker**: Deploy clustering model as a REST API for automated health risk scoring
- **Google BigQuery**: Store and query population-scale activity data
- **Azure Data Factory / AWS Glue**: ETL pipelines for wearable device data ingestion
- **Power BI Service**: Publish interactive dashboards with row-level security
- **MLflow**: Track model experiments, versions, and performance metrics
- **Azure Databricks / PySpark**: Process large-scale wearable data streams

---

## 🏗️ Real-World Applications

| Domain | Application |
|--------|-------------|
| **Healthcare** | Population health risk stratification and intervention targeting |
| **Insurance** | Wellness-based premium adjustments using activity data |
| **Retail (Wellness)** | Personalized product recommendations for fitness/health products |
| **Corporate HR** | Employee wellness programme design and ROI measurement |
| **Public Health** | Policy evaluation for national physical activity guidelines |
| **Wearable Tech** | User segmentation for feature prioritization and engagement |

---

## 🚀 How to Run

```bash
# Clone the repository
git clone https://github.com/tayoasaolu/physical-activity-dashboard.git
cd physical-activity-dashboard

# Install dependencies
pip install -r requirements.txt

# Run the dashboard
python physical_activity_dashboard.py

---

**## requirements.txt**
pandas>=1.5.0
numpy>=1.23.0
matplotlib>=3.6.0
seaborn>=0.12.0
scipy>=1.9.0
scikit-learn>=1.1.0

📂 Repository Structure
physical-activity-dashboard/
├── README.md
├── requirements.txt
├── physical_activity_dashboard.py
├── physical_activity_dashboard.png
├── physical_activity_dashboard.pdf
├── clustering_health_risk.png
└── data/
    └── physical_activity.csv


👤 About the Author
Olutayo Daniel Asaolu — Data Analyst & Data Scientist with 8+ years of
experience in retail/FMCG analytics, specializing in translating complex datasets
into actionable business insights.

🔗 LinkedIn
🌐 Portfolio
📧 olutayoasaolu@gmail.com


📜 License
MIT License — feel free to use, modify, and share with attribution.

Built for the #SIAnalytics7DayDataVizChallenge | Day 1

---
