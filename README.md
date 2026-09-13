# Student Performance Analysis using Python & Pandas

![Python](https://img.shields.io/badge/Python-3.x-blue?logo=python)
![NumPy](https://img.shields.io/badge/NumPy-Data%20Analysis-orange?logo=numpy)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458?logo=pandas)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626?logo=jupyter)

## Overview

This project explores **student academic performance** using Python, NumPy, and Pandas.

The analysis works with a large student dataset containing **1,000,000 records and 6 core variables**, covering:

* Weekly self-study hours
* Attendance percentage
* Class participation
* Total score
* Grade
* Student ID

The objective is to practice data analysis techniques on a realistic education-focused dataset while answering practical questions about student study patterns and academic performance.

---

## Project Objectives

The project focuses on understanding student performance through questions such as:

* How large is the dataset?
* Which student studies the most each week?
* Which students have the highest attendance?
* Which students have the highest class participation?
* Which students achieve the highest total scores?
* How many students scored exactly 100?
* How can students be classified based on their performance?
* How can study efficiency be measured?
* How can students be grouped according to weekly study hours?

---

## Dataset

The dataset contains **1,000,000 student records** and the following six original columns:

| Column                    | Description                        |
| ------------------------- | ---------------------------------- |
| `student_id`              | Unique student identifier          |
| `weekly_self_study_hours` | Hours spent on self-study per week |
| `attendance_percentage`   | Student attendance percentage      |
| `class_participation`     | Class participation score          |
| `total_score`             | Overall student score              |
| `grade`                   | Assigned academic grade            |

## The notebook later creates additional analytical columns such as `ScoringLevel`, `efficiency`, and `Category`.

## Tools & Technologies

| Tool                 | Purpose                          |
| -------------------- | -------------------------------- |
| **Python**           | Programming and data analysis    |
| **NumPy**            | Numerical operations             |
| **Pandas**           | Data manipulation and analysis   |
| **Jupyter Notebook** | Interactive analysis environment |

---

# Analysis Workflow

## 1. Data Loading

The dataset is imported into Pandas using:

```python
df = pd.read_csv('student_performance.csv')
```

NumPy and Pandas are used as the main analytical libraries.

---

## 2. Dataset Exploration

The project begins with basic dataset exploration, including:

* Dataset dimensions
* First 10 records
* Last 10 records
* Column names
* Basic student-level inspection

The dataset contains exactly **1,000,000 rows and 6 columns**.

---

# Student Performance Analysis

## Weekly Self-Study

The project identifies the maximum weekly self-study time and students achieving that value.

The maximum observed self-study time is **40 hours per week**, with **166 students** reaching that value in the analysis.
A ranking of students by weekly study hours is also created using Pandas sorting.

---

## Attendance Analysis

The notebook identifies students with the maximum attendance percentage.

The highest attendance value observed is **100%**, and the analysis returns all students achieving that maximum.

This demonstrates how filtering can be used to find all records matching an extreme value rather than returning only one student.

---

## Class Participation

The project also investigates the highest class participation score.

The maximum participation value is **10.0**, and the notebook filters all students who achieve that score.
This shows practical use of:

```python
max()
```

and Boolean filtering in Pandas.

---

## Total Score Analysis

Students are analyzed according to their total academic score.

The maximum total score is **100.0**, and the notebook identifies all students who achieved that score.
The analysis also calculates how many students scored exactly 100.

### Students scoring 100: **268,121**

---

# Derived Features

## Scoring Level

A new `ScoringLevel` column is created using custom conditional logic.

The defined categories are:

* **High:** Total score ≥ 90
* **Medium:** 70 ≤ Total score < 90
* **Low:** 50 ≤ Total score < 70

The classification is implemented through a Python function and Pandas `apply()`.

---

## Study Efficiency

The notebook creates a new metric:

```text
Study Efficiency = Total Score / Weekly Self-Study Hours
```

This is implemented using direct Pandas column arithmetic.

The metric provides a way to compare academic score relative to the amount of weekly self-study recorded.

---

## Study Category

Students are grouped into three study-intensity categories based on weekly self-study hours:

| Category     | Weekly Study Hours |
| ------------ | -----------------: |
| **Light**    |               < 10 |
| **Moderate** |              10–20 |
| **Heavy**    |               > 20 |

This classification is implemented using a custom function and `apply()`.

---

# Key Analytical Takeaways

### 1. Large-Scale Dataset

The project demonstrates Pandas analysis on a dataset containing **one million student records**, making it useful practice for working with larger-than-usual tabular datasets.

### 2. Study Time Can Be Analyzed at Individual Level

Students can be ranked and filtered based on weekly self-study hours, with 40 hours being the maximum observed value.

### 3. Attendance Can Be Used as a Performance Attribute

The notebook identifies all students reaching the highest observed attendance level of 100%.

### 4. Maximum Scores Are Common in This Dataset

A substantial number of records have a total score of exactly 100, with **268,121 students** meeting that condition.

### 5. Derived Metrics Add Analytical Depth

## Creating `Study Efficiency`, `ScoringLevel`, and `Category` moves the analysis beyond simply inspecting the raw columns.

# Pandas Concepts Demonstrated

This project provides hands-on practice with:

* `read_csv()`
* `shape`
* `head()`
* `tail()`
* `columns`
* `max()`
* Boolean filtering
* `sort_values()`
* Column creation
* Custom functions
* `apply()`
* Conditional classification
* Arithmetic between DataFrame columns

---

# Project Structure

```text
Student-Per
```

