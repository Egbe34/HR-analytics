# HR Analytics 

A fast, portfolio-ready HR analytics project you can push to GitHub **right now**. It includes a synthetic employee dataset, KPI analysis, clean matplotlib charts, and a simple attrition (churn) model.

## What's Inside
- **data/hr_employees.csv** – synthetic HR dataset (600 rows)
- **src/analyze.py** – one-click analysis: KPIs, charts, and a logistic regression model
- **outputs/** – auto-generated figures and reports
- **requirements.txt** – minimal dependencies
- **MIT License** – safe for public use

## Quick Start
```bash
# 1) Create & activate a virtual env (optional but recommended)
python -m venv .venv
# Windows: .venv\Scripts\activate
# macOS/Linux: source .venv/bin/activate

# 2) Install deps
pip install -r requirements.txt

# 3) Run analysis
python src/analyze.py
```

Outputs will appear in `outputs/`:
- `kpi.json` – headcount & attrition rates (overall/by group)
- `attrition_by_department.png`
- `income_by_attrition.png`
- `years_vs_income.png`
- `model_report.txt` – precision/recall/F1 and confusion matrix
- `top_feature_coefficients.csv` – most predictive features

## Example KPIs (from the synthetic data)
- Headcount: ~600
- Overall Attrition Rate: ~15–25%
- Highest Attrition by Department typically in Sales / R&D (varies per seed)

> Note: The dataset is synthetic but realistic. You can swap in your own HR CSV using the same columns to re-run the analysis.

## Project Structure
```
hr-analytics-quickstart/
├─ data/
│  └─ hr_employees.csv
├─ outputs/
├─ src/
│  └─ analyze.py
├─ .gitignore
├─ LICENSE
├─ requirements.txt
└─ README.md
```

## Use Cases
- Portfolio showcase (EDA + ML)
- Quick baseline for HR dashboards
- Teaching/demo material

## License
MIT – do anything, credit appreciated.
