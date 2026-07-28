# 👥 HR Attrition & Workforce Analytics Dashboard | Power BI

## 📌 Project Overview
This project is an interactive Power BI dashboard built to analyze employee 
attrition using the IBM HR Analytics dataset. It combines Python-based data 
cleaning with Power BI visualization to identify which employee segments are 
most at risk of leaving, supporting data-driven retention strategy.

## 📊 Dashboard Pages

### Page 1
A high-level view of workforce attrition across department, tenure, and role.

**KPIs Included:**
- Total Employees
- Attrition Count
- Attrition Rate
- Average Tenure
- Average Satisfaction

**Visuals:**
- Attrition Rate by Department
- Attrition Rate by TenureBucket
- Attrition Rate by JobRole
- Interactive Department & TenureBucket Filters

### Page 2
Deeper segmentation by behavioral and demographic factors, plus a combined 
risk matrix.

**Visuals:**
- Attrition Rate by OverTime
- Attrition Rate by Gender
- Attrition Rate by MaritalStatus
- Attrition Rate by JobSatisfaction
- Average MonthlyIncome by Attrition
- TenureBucket × JobSatisfaction Risk Matrix
- Interactive Gender, OverTime & JobRole Filters

## 📚 DAX Measures Used
- Total Employees
- Attrition Count
- Attrition Rate
- Avg Satisfaction
- Avg Tenure

**Calculated Columns (Python)**
- TenureBucket — binned from YearsAtCompany (`<2 years`, `2-5 years`, 
  `5-10 years`, `10+ years`)

## 🛠 Tools Used
- Power BI Desktop
- Power Query
- DAX (Data Analysis Expressions)
- Python (Pandas) — data validation and feature engineering

## 📂 Dataset
- **Source:** [IBM HR Analytics Employee Attrition & Performance — Kaggle](https://www.kaggle.com/datasets/pavansubhasht/ibm-hr-analytics-attrition-dataset)
- **Scope:** 1,470 employee records, no missing values across any field 
  (validated in Python)
- Feature engineering (tenure bucketing) performed in Python/Pandas before 
  loading into Power BI

## 📷 Dashboard Screenshots
The `/screenshots` folder contains images of every dashboard page.
- Page 1
- Page 2

## 💡 Key Insights
- **Total Employees:** 1,470
- **Overall Attrition Rate:** 16.1%
- **Average Tenure:** 7.01 years
- **Average Satisfaction:** 2.72 / 4

The dashboard reveals:
- **Tenure is a strong attrition driver** — employees with under 2 years 
  tenure leave at 29.8%, nearly 4x the rate of employees with 10+ years (8.1%)
- **Role-specific risk** — Sales Representatives show the highest attrition 
  of any role at 39.8%, more than double the next-highest role
- **Overtime is the strongest behavioral predictor** — employees working 
  overtime leave at 30.5% vs. 10.4% for those who don't, roughly a 3x difference
- **Pay gap between leavers and stayers** — employees who left earned an 
  average of $4.8K/month vs. $6.8K for those who stayed
- **Compounding risk factor (verified via Python):** employees with <2 years 
  tenure AND low job satisfaction represent only 8.6% of the workforce but 
  account for 19.4% of all attrition — a 2.2x overrepresentation. This 
  segment peaks at a 41.9% attrition rate in the risk matrix, nearly 4x the 
  overall average.

## ⭐ Key Features
- Interactive slicers (Department, TenureBucket, Gender, OverTime, JobRole)
- KPI Cards
- Dynamic DAX Measures
- TenureBucket × JobSatisfaction Risk Matrix
- Python-validated data cleaning and feature engineering
- Data-Driven Insight Callouts

## 🚀 Skills Demonstrated
- Power BI
- Python (Pandas)
- Data Cleaning & Validation
- Feature Engineering
- DAX
- Power Query
- KPI Design
- Dashboard Design
- Interactive Filtering
- Data Visualization
- Workforce Analytics

## 📌 Author
Vaishnavi Chedudhupu
Aspiring Data Analyst
