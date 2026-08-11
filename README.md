# Home Health Quality Performance Analytics

### Medicare Home Health Patient Experience | Healthcare Operations & Executive Analytics

Transforming Medicare Home Health patient-experience data into actionable operational insights through **healthcare analytics, exploratory machine learning, scenario modeling, and business intelligence**.

This project analyzes state-level Medicare Home Health quality data to identify operational measures associated with patient satisfaction and demonstrate how analytics can support healthcare quality-improvement and executive decision-making.

---

## Executive Dashboard

![Home Health Quality Executive Dashboard](images/executive_dashboard.png)

*Interactive Tableau dashboard for monitoring patient satisfaction, recommendation rates, professional care performance, and survey volume across states.*

---

## Professional Project Report

A management-ready summary of the analytical methodology, key findings,
scenario analysis, business recommendations, and responsible interpretation.

[View the Professional Analytics Report](reports/Home_Health_Quality_Analytics_Professional_Report.pdf)

---

## Project Overview

Healthcare organizations continuously monitor patient experience and quality measures to identify performance gaps, improve care delivery, and support operational decision-making.

This project evaluates Medicare Home Health patient survey data to identify operational factors associated with overall patient satisfaction.

The project demonstrates an end-to-end healthcare analytics workflow including:

- Data Quality Assessment
- Exploratory Data Analysis
- Statistical Relationship Analysis
- Exploratory Machine Learning
- Sensitivity Testing
- Operational Scenario Modeling
- Tableau Business Intelligence
- Executive Decision Support

Rather than focusing solely on predictive modeling, this project emphasizes **translating healthcare quality data into actionable operational insights for healthcare leaders**.

---

## Business Questions

1. Which quality metrics are most strongly associated with overall patient satisfaction?
2. Which operational areas should healthcare organizations prioritize to improve quality ratings?
3. Can machine learning identify important operational features associated with healthcare performance?
4. How can analytics support executive decision-making?

---

## Key Findings

Across multiple analytical approaches, **Communication** and **Professional Care** consistently emerged as the strongest operational signals associated with overall patient satisfaction.

### Relationship Analysis

- **Professional Care** demonstrated the strongest direct relationship with Patient Rating (**r = 0.982**).
- **Communication** also demonstrated a very strong relationship with Patient Rating (**r = 0.964**).

### Exploratory Machine Learning

Leave-one-state-out sensitivity testing of the Random Forest feature rankings produced:

| Operational Feature | Mean Importance |
| --- | ---: |
| Communication | **0.312** |
| Professional Care | **0.262** |
| Pain Medicines & Home Safety | 0.230 |
| Response Rate | 0.110 |
| Completed Surveys | 0.085 |

Communication ranked highest on average, while Professional Care demonstrated particularly stable importance across sensitivity iterations.

### Operational Scenario Analysis

Using observed 75th-percentile performance values as improvement benchmarks:

| Scenario | Predicted Patient Rating | Change vs. Baseline |
| --- | ---: | ---: |
| Baseline | 84.60% | — |
| Improve Communication | **85.30%** | **+0.70 pp** |
| Improve Professional Care | 84.79% | +0.19 pp |
| Improve Both | **85.48%** | **+0.88 pp** |

Improving Communication produced the largest individual modeled improvement, while improving **Communication and Professional Care together** produced the strongest overall scenario result.

> **Interpretation:** These findings identify data-informed areas for further quality-improvement evaluation. Because the analysis contains only 10 state-level observations, the machine-learning and scenario results are exploratory and should not be interpreted as causal or production-ready predictions.

---

## Project Workflow

```text
Medicare Home Health Survey Data
              │
     Data Quality Review
              │
 Exploratory Data Analysis
              │
   Relationship Analysis
              │
Exploratory Machine Learning
              │
     Sensitivity Testing
              │
 Operational Scenario Analysis
              │
 Executive Recommendations
              │
 Tableau Executive Dashboard
```

---

## Tools & Technologies

| Category | Technologies |
| --- | --- |
| Programming | Python |
| Data Analysis | Pandas, NumPy |
| Machine Learning | Scikit-learn |
| Visualization | Matplotlib, Tableau |
| Development | Jupyter Notebook |
| Data Source Format | Microsoft Excel |
| Version Control | Git & GitHub |

### Analytical Techniques

- Exploratory Data Analysis (EDA)
- Data Quality Assessment
- Correlation Analysis
- Random Forest Regression
- Feature Importance Analysis
- Leave-One-State-Out Sensitivity Testing
- Operational Scenario Modeling
- Executive Dashboard Development

---

## Business Impact

The analysis suggests that **Communication should be considered a primary improvement priority, supported by continued focus on Professional Care**.

Potential operational areas for further evaluation include clearer patient education, consistent care-plan communication, responsiveness to patient questions, and reinforcement of patient-centered communication practices.

The Tableau Executive Dashboard extends the analysis into an interactive decision-support environment, allowing healthcare leaders to monitor patient satisfaction, recommendation rates, professional care performance, and survey volume across states.

---

## Repository Structure

```text
Home-Health-Quality-Analytics/
README.md
.gitignore
    data/
        Home Health Care Patient Survey State Data.xlsx
    notebooks/
        Healthcare_Quality_Analytics_Portfolio.ipynb
    dashboards/
        Home_Health_Quality_Executive_Dashboard.twb
    images/
        executive_dashboard.png
    documentation/
        Analysis_Inventory.docx
        Project_Vision.docx
    reports/
      Home_Health_Quality_Analytics_Professional_Report.pdf
```

---

## About the Author

### Angeline Duarte

**Healthcare Operations & Technology | Systems Analysis | Data Analytics**

This repository is part of my professional portfolio showcasing healthcare analytics, business intelligence, machine learning, and healthcare technology projects.

- Portfolio: [Click Here](https://www.angelineduarte.com/)
- LinkedIn: [Click Here](https://www.linkedin.com/in/angelineduarte/)

---

If you found this project interesting, feel free to explore the repository or connect with me on LinkedIn.
