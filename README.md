[README (8).md](https://github.com/user-attachments/files/31862310/README.8.md)
# Reducing Employee Turnover: An HR Analytics Dashboard for Workforce Retention

An HR analytics dashboard analyzing employee attrition drivers, built on a synthetic dataset modeled to reflect realistic Nigerian workforce patterns, and benchmarked against reported Nigerian banking-sector turnover figures.

## Business Problem

Employee turnover is expensive — in lost productivity, rehiring costs, and institutional knowledge. This project simulates a mid-sized organization (1,500 employees across 8 departments) to answer a practical question: **which specific, addressable factors are driving people to leave, and where should retention efforts focus first?**

Rather than presenting turnover as one flat number, the dashboard breaks it down by department, tenure, overtime status, promotion history, and job satisfaction — then ties each finding to a concrete recommendation.

## Dashboard Pages

### 1. Overview
![Overview](screenshots/01-overview.png)
Headline attrition rate (30.3%), total headcount, cost-of-turnover estimate, and a benchmark callout comparing the result against Nigeria's banking-sector turnover trend (~28%, 2021).

### 2. Attrition Drivers — "Two Moments Decide Who Stays"
![Attrition Drivers](screenshots/02-attrition-drivers.png)
Breaks down attrition by tenure, years since last promotion, job satisfaction, and department × overtime status. Two findings stand out: attrition peaks in the first year (37.1%) and spikes again sharply at the 3-year promotion mark (37.4%).

### 3. Workforce Composition — "Growing, But Still Leaking Talent"
![Workforce Composition](screenshots/03-workforce-composition.png)
Hiring and exit trends over time, hiring source effectiveness, and demographic composition (gender by department, age distribution). Headcount has grown steadily while exits have stayed relatively flat.

### 4. Recommendations
![Recommendations](screenshots/04-recommendations.png)
Five data-backed recommendations, each tied directly to a specific finding from the earlier pages — not generic HR advice.

## Key Findings

- **Overall attrition (30.3%)** is broadly in line with Nigeria's banking-sector turnover benchmark (~28%, 2021)
- **Overtime nearly doubles attrition risk** — 63.9% for staff working overtime vs. 36.1% for others; the strongest single driver identified
- **New hires are the highest flight risk** — 37.1% attrition in year one vs. 26.2% for employees with 7+ years of tenure
- **Attrition spikes sharply at the 3-year promotion mark** (37.4%), suggesting a specific "stall point" rather than a steady climb
- **Marketing and Finance** run 4+ points above the company average (35.5%, 34.6%)
- **Job satisfaction is a weak predictor of attrition** (3.0 for leavers vs. 3.5 for stayers) — structural factors (overtime, tenure, promotion gaps) matter more than morale scores alone
- **Employee Referral is the top hiring channel** (324 hires, ahead of Job Board's 295)
- The workforce skews young — 77% of employees are under 35

## Tools Used

- **Power BI** — dashboard build, DAX measures, data modeling
- **Python (pandas)** — synthetic dataset generation with embedded realistic attrition patterns
- **Excel** — data dictionary and benchmark documentation

## A Note on the Dataset

The dataset is synthetic — built with Python to reflect realistic HR patterns rather than pulled from a public Kaggle dataset. Attrition was modeled as a function of overtime, satisfaction, tenure, promotion gap, pay, and commute distance, so the correlations found in the dashboard reflect genuine embedded signal rather than random noise. Its overall attrition rate was sanity-checked against Nigeria's banking-sector turnover figures as a directional reference, not a precise validation (see the Benchmarks tab in the dataset file for sourcing).

## Files

- `HR_Retention_Dataset.xlsx` — synthetic dataset, data dictionary, and benchmark sources
- `HR_Dashboard.pbix` — full Power BI dashboard
- `/screenshots` — page-by-page exports

---
Built by Oluwabusola Oyenuga · [LinkedIn] · [Portfolio]
