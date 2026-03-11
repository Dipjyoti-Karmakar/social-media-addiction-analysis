# Social Media Addiction Analysis

<p align="center"><strong>Data-driven EDA and storytelling on student social media behavior, academic impact, and addiction risk patterns.</strong></p>

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.10+-3776AB?style=for-the-badge&logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/Pandas-EDA-150458?style=for-the-badge&logo=pandas&logoColor=white" />
  <img src="https://img.shields.io/badge/Seaborn-Visualization-4C72B0?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Jupyter-Notebook-F37626?style=for-the-badge&logo=jupyter&logoColor=white" />
  <img src="https://img.shields.io/badge/Power%20BI-Dashboard-F2C811?style=for-the-badge&logo=powerbi&logoColor=black" />
  <img src="https://img.shields.io/badge/Status-Completed-2ea44f?style=for-the-badge" />
</p>

---

## Executive Summary

This project analyzes student social media usage data to understand addiction trends and their relationship with academic performance, sleep, and interpersonal conflicts.

The analysis combines data cleaning, exploratory visualizations, grouped insights, and simple rule-based risk classification to produce clear findings and a reporting-ready dashboard output.

## Overview

The workflow:
1. Load and validate student behavior data
2. Check data quality (nulls, duplicates, data types)
3. Perform exploratory data analysis and relationship plots
4. Aggregate metrics by gender, age, and academic level
5. Classify risk level and suggest digital detox actions
6. Build a storytelling output for reporting

### Key Outcomes

- Female students show slightly higher average addiction scores than male students
- Students aged 19 to 20 show high daily usage concentration
- High school students show the highest average addiction score among academic groups
- More social media conflict aligns with lower sleep duration and weaker academic outcomes
- The project includes both notebook analysis and a Power BI dashboard artifact

---

## Architecture

**Data Flow**

```
CSV Dataset (data/)
        ↓
Data Cleaning + Validation (Notebook)
        ↓
Exploratory Analysis + Visual Insights
        ↓
Aggregations + Risk Logic
        ↓
Storytelling + Dashboard Output (reports/)
```

---

## How to get the code

```bash
git clone https://github.com/Dipjyoti-Karmakar/social-media-addiction-analysis.git
```

## Project Structure

```
Social-Media-Addiction-Analysis/
│
├── data/
│   └── student_addiction_data.csv
│
├── notebooks/
│   └── social_media_addiction_analysis.ipynb
│
├── reports/
│   ├── addiction_analysis_dashboard.pbix
│   ├── Screenshot 2026-03-10 230939.png
│   ├── Screenshot 2026-03-10 231033.png
│   ├── Screenshot 2026-03-10 231058.png
│   ├── Screenshot 2026-03-10 231112.png
│   └── Screenshot 2026-03-10 231127.png
│
├── README.md
├── run_notebook.md
├── requirements.txt
└── .gitignore
```

---

## Methodology

| Phase | Tools | Purpose |
|-------|-------|---------|
| Ingestion | pandas | Load and inspect student dataset |
| Validation | pandas | Check nulls, duplicates, and schema |
| EDA | matplotlib, seaborn | Analyze distributions and relationships |
| Aggregation | pandas, NumPy | Compare grouped patterns by demographics |
| Rule-Based Logic | Python | Assign risk level and suggest detox strategy |
| Reporting | Power BI | Build shareable visual dashboard |

---

## Data Dictionary

- `Student_ID`: Unique identifier for each student record
- `Age`: Age of the student
- `Gender`: Student gender
- `Academic_Level`: Education stage (High School, Undergraduate, Graduate)
- `Country`: Student country
- `Avg_Daily_Usage_Hours`: Average daily social media usage in hours
- `Most_Used_Platform`: Primary social media platform used
- `Affects_Academic_Performance`: Whether social media usage affects academics (Yes/No)
- `Sleep_Hours_Per_Night`: Average sleep duration per night
- `Mental_Health_Score`: Self-reported mental health score
- `Relationship_Status`: Relationship status category
- `Conflicts_Over_Social_Media`: Number of conflicts caused by social media use
- `Addicted_Score`: Composite addiction score used in this analysis

---

## Dashboard Preview

<p align="center">
        <img src="./reports/Screenshot 2026-03-10 231414.png" width="90%" alt="Dashboard View 1" />
</p>

<p align="center">
        <img src="./reports/Screenshot 2026-03-10 231427.png" width="90%" alt="Dashboard View 2" />
</p>

<p align="center">
        <img src="./reports/Screenshot 2026-03-10 231439.png" width="90%" alt="Dashboard View 3" />
</p>

<p align="center">
        <img src="./reports/Screenshot 2026-03-10 231451.png" width="90%" alt="Dashboard View 4" />
</p>

<p align="center">
        <img src="./reports/Screenshot 2026-03-10 231509.png" width="90%" alt="Dashboard View 5" />
</p>

### Insights From Dashboard Views

- Demographic splits in the dashboard reinforce that addiction levels are not uniform across gender and academic level groups.
- Usage-hour patterns and addiction-score visuals consistently point to late-teen and early-20s cohorts as higher-risk segments.
- Cross-view comparisons indicate that higher daily usage is associated with lower sleep hours and weaker academic outcomes.
- Conflict-based panels align with the notebook observation that interpersonal friction rises with higher addiction intensity.
- Platform-level comparisons support targeted intervention strategy design rather than one-size-fits-all recommendations.

---

## Quick Start

```bash
cd Social-Media-Addiction-Analysis

python -m venv .venv
.venv\Scripts\activate   # Windows

pip install -r requirements.txt

jupyter notebook notebooks/social_media_addiction_analysis.ipynb
```

## Notebook Execution Note

The notebook loads data using a relative path (`../data/student_addiction_data.csv`) from inside `notebooks/social_media_addiction_analysis.ipynb`.

If you launch Jupyter from the repository root using the command above, this path resolves correctly.

---

## Tech Stack

Python • pandas • NumPy • Matplotlib • Seaborn • Jupyter • Power BI

---

## Author

**Your Name**  
Data Analyst | Python • EDA • Dashboarding
