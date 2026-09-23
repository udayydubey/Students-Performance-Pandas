# Student Performance Analysis — Python & Pandas

![Python](https://img.shields.io/badge/Python-3.x-blue?logo=python)
![NumPy](https://img.shields.io/badge/NumPy-Analysis-orange?logo=numpy)
![Pandas](https://img.shields.io/badge/Pandas-Analysis-150458?logo=pandas)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626?logo=jupyter)

> A practical Pandas project analyzing **1,000,000 student records** to explore academic performance, study behavior, attendance, participation, and derived performance metrics.

## Overview

This project uses Python, NumPy, and Pandas to answer practical questions about student performance while demonstrating core data-analysis techniques on a large tabular dataset.

### Business-style questions

- Which students study the most?
- Which students have the highest attendance and participation?
- How many students achieved a perfect score?
- How can students be classified by performance?
- How can study intensity and study efficiency be measured?

## Dataset

The dataset contains **1,000,000 rows and 6 original columns**:

| Column | Description |
|---|---|
| `student_id` | Unique student identifier |
| `weekly_self_study_hours` | Weekly self-study hours |
| `attendance_percentage` | Attendance percentage |
| `class_participation` | Participation score |
| `total_score` | Overall score |
| `grade` | Academic grade |

## Analysis Workflow

**Load → Inspect → Filter → Sort → Transform → Derive Metrics → Categorize → Interpret**

### Core analysis

- Dataset shape and structure
- Maximum study hours
- Highest attendance
- Highest participation
- Maximum total score
- Students scoring exactly 100
- Ranking and Boolean filtering

### Derived features

**ScoringLevel**
- High: score ≥ 90
- Medium: 70–89
- Low: 50–69

**Study Efficiency**

`Study Efficiency = Total Score / Weekly Self-Study Hours`

**Study Category**
- Light: < 10 hours
- Moderate: 10–20 hours
- Heavy: > 20 hours

## Key Results

- Maximum observed self-study time: **40 hours/week**
- Students at that maximum: **166**
- Maximum attendance: **100%**
- Maximum participation: **10.0**
- Maximum total score: **100**
- Students scoring 100: **268,121**

These results describe this dataset and should not be interpreted as general conclusions about student performance.

## Pandas Concepts Demonstrated

- `read_csv()`
- `shape`
- `head()` / `tail()`
- `columns`
- `max()`
- Boolean filtering
- `sort_values()`
- Column creation
- Custom functions
- `apply()`
- Conditional classification
- DataFrame column arithmetic

## Project Structure

```text
Students-Performance-Pandas/
├── README.md
├── student_performance.csv
└── *.ipynb
```

## How to Run

```bash
pip install pandas numpy jupyter
jupyter notebook
```

Open the project notebook and run the cells sequentially.

## Skills Demonstrated

**Python • NumPy • Pandas • Data Manipulation • Feature Engineering • Exploratory Analysis • Jupyter**

---

### Author

**Uday Dubey**  
BBA Student | Aspiring Data Analyst

[GitHub](https://github.com/udayydubey)

⭐ If you found the project useful, feel free to star the repository.
