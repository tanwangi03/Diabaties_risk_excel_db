# 🩺 Diabetes Patient Analysis Dashboard

> **Better Data | Healthier Lives | A Stronger Tomorrow**

An interactive healthcare analytics dashboard designed to analyze diabetes risk across a patient population using demographic, lifestyle, family-history, and clinical health indicators.

## 📌 Project Overview

The **Diabetes Patient Analysis Dashboard** transforms patient-level healthcare data into an interactive and visually intuitive analytical report.

The dashboard focuses on understanding how demographic, lifestyle, behavioral, and clinical factors relate to diabetes risk. It enables users to explore patient segments, compare risk categories, identify geographic patterns, and understand how key clinical indicators vary across risk levels.

The dashboard analyzes **15,000 patients** across three risk categories:

| Risk Level | Patients | Percentage |
|---|---:|---:|
| 🟢 Low Risk | 9,000 | 60% |
| 🟡 Moderate Risk | 3,750 | 25% |
| 🔴 High Risk | 2,250 | 15% |
| **Total** | **15,000** | **100%** |

## 🎯 Objectives

- Analyze the overall distribution of diabetes risk.
- Compare diabetes risk across physical activity levels.
- Examine the relationship between family history and diabetes risk.
- Identify cities with the highest number of high-risk patients.
- Compare fasting blood sugar and HbA1c across risk categories.
- Provide interactive filtering for focused patient analysis.
- Communicate healthcare insights through clear visualizations.

## 🖥️ Dashboard Preview

![Diabetes Patient Analysis Dashboard](images/dashboard-overview.png)

*Complete dashboard showing KPIs, risk distribution, lifestyle analysis, geographic analysis, clinical indicators, filters, and key insights.*

## 📊 Dashboard KPIs

| KPI | Value |
|---|---:|
| Total Patients | **15,000** |
| High Risk Patients | **2,250 (15%)** |
| Moderate Risk Patients | **3,750 (25%)** |
| Low Risk Patients | **9,000 (60%)** |

## 📈 Dashboard Analysis

### 1. Distribution of Patients by Diabetes Risk Level

![Patient Risk Distribution](images/risk-distribution.png)

The doughnut chart shows the overall distribution of patients across Low, Moderate, and High diabetes-risk categories. Low Risk is the largest segment at **60%**, followed by Moderate Risk at **25%** and High Risk at **15%**.

### 2. Physical Activity Level vs Diabetes Risk

![Physical Activity vs Diabetes Risk](images/activity-risk.png)

This stacked-column chart compares risk levels across **Active, Moderate, and Sedentary** activity groups. The dashboard shows the highest displayed High-Risk proportion among sedentary individuals at **25%**.

### 3. Family History vs Diabetes Risk

![Family History vs Diabetes Risk](images/family-history-risk.png)

The dashboard compares patients with and without a family history of diabetes.

| Family History | Low Risk | Moderate Risk | High Risk |
|---|---:|---:|---:|
| Yes | 45% | 30% | 25% |
| No | 75% | 18% | 7% |

The displayed analysis shows a higher High-Risk proportion among patients reporting a family history.

### 4. Cities with Highest High-Risk Patients

![Cities with Highest High-Risk Patients](images/city-risk.png)

The geographic analysis ranks cities by the number of High-Risk patients.

| City | High-Risk Patients |
|---|---:|
| Mumbai | 420 |
| Delhi | 380 |
| Bengaluru | 310 |
| Hyderabad | 260 |
| Chennai | 210 |
| Kolkata | 180 |
| Pune | 150 |
| Ahmedabad | 120 |

**Mumbai** has the highest displayed number of High-Risk patients.

### 5. Average Blood Sugar & HbA1c by Risk Level

![Blood Sugar and HbA1c Analysis](images/clinical-risk.png)

The chart compares average fasting blood sugar and HbA1c across risk groups.

| Risk Level | Avg. Fasting Blood Sugar (mg/dL) | Avg. HbA1c (%) |
|---|---:|---:|
| Low Risk | 92 | 5.2 |
| Moderate Risk | 118 | 6.8 |
| High Risk | 162 | 8.9 |

Both displayed clinical measures increase with higher diabetes-risk level.

## 🎛️ Interactive Filters

![Dashboard Filters](images/filters.png)

The dashboard provides filters for:

- Gender
- Age Group
- City
- Physical Activity Level
- Family History
- Diabetes Risk

These controls allow users to focus on specific patient segments and explore how risk patterns change.

## 💡 Key Insights

![Key Insights](images/key-insights.png)

1. **Low Risk is the largest patient segment**, representing 60% of the population.
2. **Sedentary individuals show the highest displayed High-Risk proportion**, at 25%.
3. **Family history is associated with a higher displayed High-Risk proportion**: 25% with family history versus 7% without.
4. **Mumbai has the highest displayed High-Risk patient count**, with 420 patients.
5. **Average fasting blood sugar and HbA1c increase across risk levels**, reaching 162 mg/dL and 8.9% respectively in the High-Risk group.

## 🗂️ Dataset Overview

Each row represents an individual patient.

| Column | Description |
|---|---|
| `patient_id` | Unique patient identifier |
| `age` | Patient age in years |
| `gender` | Patient gender |
| `city` | Patient's city |
| `bmi` | Body Mass Index |
| `family_history_diabetes` | Family history of diabetes |
| `physical_activity_level` | Active, Moderate, or Sedentary |
| `diet_type` | Dietary category |
| `smoking_status` | Smoking-status category |
| `alcohol_consumption` | Alcohol-consumption category |
| `hours_sleep_per_night` | Average sleep duration |
| `stress_level` | Reported stress level |
| `fasting_blood_sugar` | Fasting blood sugar in mg/dL |
| `hba1c_level` | HbA1c level in % |
| `blood_pressure_systolic` | Systolic blood pressure in mmHg |
| `blood_pressure_diastolic` | Diastolic blood pressure in mmHg |
| `waist_circumference_cm` | Waist circumference in centimeters |
| `income_bracket` | Patient income category |
| `diabetes_risk` | Final diabetes-risk classification |

## 🔎 Sample Data

| Patient ID | Age | Gender | City | BMI | Family History | Activity | Fasting Sugar | HbA1c | Risk |
|---:|---:|---|---|---:|---|---|---:|---:|---|
| 1 | 47 | Female | Mumbai | 26.5 | Yes | Sedentary | 178 | 7.3 | Low |
| 2 | 53 | Female | Mumbai | 20.5 | Yes | Moderate | 152 | 6.9 | Low |
| 3 | 47 | Male | Thane | 31.3 | No | Moderate | 168 | 6.6 | High |
| 8 | 42 | Female | Delhi | 19.5 | No | Active | 270 | 8.9 | High |
| 10 | 44 | Male | Mumbai | 24.1 | No | Moderate | 178 | 7.6 | Moderate |

## 🧹 Data Quality Considerations

Some sample records contain blank values, particularly for fields such as `smoking_status`, `alcohol_consumption`, and `income_bracket`.

Before advanced analysis or predictive modeling, consider:

- Handling missing values.
- Checking duplicate `patient_id` values.
- Validating numeric ranges.
- Standardizing categorical values.
- Checking for outliers.
- Validating data types and risk categories.

## 🛠️ Tools & Technologies

This project is a **healthcare analytics and data-visualization project**. Add the exact tools used in the implementation, for example:

- Power BI / Tableau
- Excel / CSV
- SQL
- Python
- Data Cleaning & Transformation
- Interactive Data Visualization

## 📁 Recommended Repository Structure

```text
Diabetes-Patient-Analysis-Dashboard/
│
├── README.md
├── data/
│   └── diabetes_patient_data.csv
├── dashboard/
│   └── dashboard-file
└── images/
    ├── dashboard-overview.png
    ├── risk-distribution.png
    ├── activity-risk.png
    ├── family-history-risk.png
    ├── city-risk.png
    ├── clinical-risk.png
    ├── filters.png
    └── key-insights.png
```

## 🚀 How to Use

1. Clone or download the repository.
2. Open the dashboard file using the required BI or visualization software.
3. Load the patient dataset.
4. Use the interactive filters to explore patient segments.
5. Review risk distribution, lifestyle patterns, geographic results, and clinical indicators.
6. Use the dashboard insights for analytical and reporting purposes.

## 📌 Project Value

This project demonstrates how healthcare data can be converted into actionable analytical insights through interactive dashboards. It combines patient segmentation, lifestyle analysis, family-history analysis, geographic comparison, and clinical indicators in one reporting interface.

Potential applications include:

- Population health analysis
- Patient-risk segmentation
- Healthcare reporting
- Lifestyle-risk analysis
- Geographic comparison
- Data analytics portfolio projects
- Interactive business-intelligence reporting

## ⚠️ Disclaimer

This dashboard is intended for **educational, analytical, and data-visualization purposes only**. The diabetes-risk classifications shown should not be considered a medical diagnosis or medical advice. Actual diagnosis and clinical risk assessment should be performed by qualified healthcare professionals using appropriate clinical evaluation.

## 👤 Author

**TANWANGI LALWANI**

**Project:** Diabetes Patient Analysis Dashboard  
**Focus:** Healthcare Analytics | Diabetes Risk Analysis | Data Visualization

---

⭐ **If you find this project useful, consider giving the repository a star!**
