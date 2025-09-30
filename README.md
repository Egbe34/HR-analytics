#  HR Analytics & Employee Management Project

This repository demonstrates an **end-to-end HR Analytics project** built with synthetic employee data.  
It shows how HR teams can use **data-driven insights** to reduce attrition, optimize workforce planning, and integrate with enterprise tools such as **Excel, SAP HR, and HRIS systems**.

---

##  Project Overview

HR Analytics is at the core of modern **Human Capital Management (HCM)**.  
This project simulates how an organization could:
- Collect **employee data** (demographics, department, income, performance, overtime, travel, satisfaction, etc.)
- Analyze **attrition trends** (why employees leave)
- Build a **predictive model** (logistic regression for attrition)
- Generate **dashboards, KPIs, and reports**
- Integrate outputs with **Excel, HRIS, or SAP SuccessFactors**

---

##  Dataset

Synthetic dataset with **600 employees**:
- Demographics: Age, Gender, Education, Marital Status  
- Work Info: Department, Job Role, Business Travel, Years at Company  
- Performance: Job Satisfaction, Performance Rating, Training  
- Compensation: Monthly Income, Overtime  
- Target Variable: **Attrition (Yes/No)**  

File: [`data/hr_employees.csv`](data/hr_employees.csv)

---

##  Tech Stack

- **Python** → data wrangling, KPIs, machine learning (scikit-learn)  
- **Matplotlib** → charts (attrition by department, income vs attrition)  
- **Excel / CSV Export** → HR can review outputs in spreadsheets  
- **SAP / HRIS Integration (Conceptual)** → outputs could feed into SAP HR or other HRIS systems  
- **Logistic Regression** → predictive attrition model with feature importance  

---

##  KPIs & Metrics

Example KPIs from the synthetic data:
- **Headcount**: ~600 employees  
- **Attrition Rate**: ~15–25%  
- **Attrition by Department**: Highest in Sales / R&D (varies per seed)  
- **Attrition by Gender**: Balanced but slightly higher in one group  
- **Attrition Factors**: Overtime, low job satisfaction, high travel frequency  

Outputs:  
- `outputs/kpi.json` → machine-readable KPIs  
- `outputs/attrition_by_department.png` → attrition per department  
- `outputs/income_by_attrition.png` → salary impact  
- `outputs/years_vs_income.png` → tenure vs income  

---

##  Predictive Modeling

- **Model Used**: Logistic Regression  
- **Accuracy**: ~75–80% (varies by random seed)  
- **Key Predictors**:
  - Overtime (Yes → higher attrition risk)  
  - Job Satisfaction (low → higher attrition)  
  - Monthly Income (lower salaries → higher attrition)  
  - Business Travel (frequent travel → higher attrition)  
  - Tenure (shorter tenure → higher attrition)  

Outputs:  
- `outputs/model_report.txt` → Precision, Recall, F1-score  
- `outputs/top_feature_coefficients.csv` → top predictors  

---

##  Visual Gallery

### Code Snippets
![Code Overview](assets/code_overview.png)  
![Model Pipeline](assets/model_pipeline.png)

### Charts
- **Attrition by Department**  
  ![Attrition by Department](outputs/attrition_by_department.png)

- **Monthly Income by Attrition**  
  ![Income by Attrition](outputs/income_by_attrition.png)

- **Years at Company vs Income**  
  ![Years vs Income](outputs/years_vs_income.png)

---

##  Real-World Applications

1. **HRIS Integration**  
   - Export model results to Excel or CSV  
   - Upload into SAP SuccessFactors, Workday, or Oracle HCM for HR dashboards  

2. **Employee Engagement**  
   - Identify at-risk employees early  
   - Deploy retention strategies (career growth, salary adjustments, flexible work policies)  

3. **Workforce Planning**  
   - Predict future attrition  
   - Align hiring strategy with expected turnover  

4. **Compensation Strategy**  
   - Use salary vs attrition analysis to optimize pay scales  

---

## 🚀 How to
