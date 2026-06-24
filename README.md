# 📊 Student Performance & Result Analysis

A complete Python data analytics project that explores what actually drives student
results — attendance, study habits, family background, and subject-wise marks —
across 600 students in Grades 9–12. Built as part of the **Naan Mudhalvan Arts
Internship Program 2026 (Python for Data Analytics track)**.

<p align="left">
  <img src="https://img.shields.io/badge/Python-3.10%2B-3776AB?logo=python&logoColor=white" alt="Python">
  <img src="https://img.shields.io/badge/Pandas-Data%20Analysis-150458?logo=pandas&logoColor=white" alt="Pandas">
  <img src="https://img.shields.io/badge/NumPy-Numerical%20Computing-013243?logo=numpy&logoColor=white" alt="NumPy">
  <img src="https://img.shields.io/badge/Matplotlib-Visualization-11557C" alt="Matplotlib">
  <img src="https://img.shields.io/badge/Jupyter-Notebook-F37626?logo=jupyter&logoColor=white" alt="Jupyter">
  <img src="https://img.shields.io/badge/Status-Completed-brightgreen" alt="Status">
  <img src="https://img.shields.io/badge/License-MIT-yellow" alt="License">
</p>

---

## 📑 Table of Contents

- [Overview](#-overview)
- [Dataset](#-dataset)
- [Project Structure](#-project-structure)
- [Key Insights](#-key-insights)
- [Visualizations](#-visualizations)
- [Tech Stack](#-tech-stack)
- [How to Run](#-how-to-run)
- [Notebook](#-notebook)
- [About This Project](#-about-this-project)
- [License](#-license)

---

## 📝 Overview

This project analyzes a dataset of **600 students** to understand the patterns
behind academic performance. Using Python, Pandas, NumPy, and Matplotlib, it
covers the full analytics workflow:

- Data generation & cleaning
- Exploratory data analysis (EDA)
- Statistical correlation analysis
- Six chart visualizations, including a combined dashboard
- Clear, data-backed insights and conclusions

> **Note:** The dataset is **synthetically generated** for this project (not real
> student records), built with realistic, correlated relationships between
> attendance, study hours, and academic outcomes so the analysis reflects
> genuine, explainable patterns.

---

## 📂 Dataset

`data/student_performance.csv` — 600 rows × 22 columns

| Column | Description |
|---|---|
| `Student_ID` | Unique student identifier |
| `Name`, `Gender`, `Age` | Basic demographics |
| `Grade`, `Section` | Class (9–12) and section (A/B/C) |
| `Attendance_%` | Attendance percentage |
| `Study_Hours_Per_Day` | Average daily study hours |
| `Parental_Education` | High School / Graduate / Post Graduate |
| `Family_Income_Level` | Low / Middle / High |
| `Internet_Access`, `Extracurricular_Activities` | Yes / No |
| `Math_Marks`, `Science_Marks`, `English_Marks`, `Social_Science_Marks`, `Computer_Science_Marks` | Subject-wise marks (out of 100) |
| `Total_Marks`, `Percentage` | Aggregate performance |
| `Grade_Letter` | A+ / A / B / C / D / F |
| `Result` | Pass / Fail |
| `Rank` | Overall rank by percentage |

---

## 🗂 Project Structure

```
student-performance-result-analysis/
│
├── data/
│   └── student_performance.csv          # Generated dataset (600 students)
│
├── charts/
│   ├── 01_subject_wise_average.png
│   ├── 02_pass_fail_distribution.png
│   ├── 03_attendance_vs_percentage.png
│   ├── 04_grade_distribution.png
│   ├── 05_study_hours_vs_percentage.png
│   └── 06_performance_dashboard.png
│
├── 01_generate_dataset.py               # Generates the synthetic dataset
├── 02_analysis.py                       # Runs full analysis + saves charts
├── 03_build_notebook.py                 # Builds the pre-run Jupyter notebook
├── Student_Performance_Analysis.ipynb   # Pre-run notebook (code + outputs)
├── requirements.txt
└── README.md
```

---

## 🔍 Key Insights

- 📈 **Attendance is the strongest predictor of performance** — a correlation
  of **0.56** between attendance and overall percentage, ahead of daily study
  hours (**0.36**).
- 💻 **Computer Science (74.8 avg)** and **English (72.8 avg)** are the
  strongest subjects; **Math (65.4 avg)** is the weakest and the clearest
  candidate for academic support.
- ✅ **96.7% of students pass overall** — but a small subset still fail
  individual subjects despite a healthy aggregate score, pointing to
  subject-specific gaps rather than across-the-board struggles.
- 🎓 Students with **post-graduate-educated parents** average **73.7%**,
  noticeably ahead of the **68.7%** average for students whose parents
  stopped at high school.
- 🏆 Top performer: **Vikram Pandian**, Grade 10, with a **100%** overall
  score.

---

## 📈 Visualizations

### 1. Performance Dashboard
A single-glance summary combining subject averages, pass/fail split,
the attendance-performance trend, and grade distribution.

![Performance Dashboard](https://raw.githubusercontent.com/hariruthranhub/student-performance-result-analysis/main/charts/06_performance_dashboard.png)

### 2. Attendance vs Overall Percentage
The clearest relationship in the entire dataset: students who attend more
consistently score meaningfully higher, with a visible upward trend line
(r = 0.56) running through the scatter of all 600 students.

![Attendance vs Percentage](https://raw.githubusercontent.com/hariruthranhub/student-performance-result-analysis/main/charts/03_attendance_vs_percentage.png)

*More charts — subject-wise averages, grade distribution, and study hours vs.
performance — are available in the [`charts/`](./charts) folder and inside the
notebook below.*

---

## 🛠 Tech Stack

- **Python 3.10+**
- **Pandas** — data manipulation and aggregation
- **NumPy** — synthetic data generation and numerical operations
- **Matplotlib** — all chart visualizations
- **Jupyter Notebook** — combined, narrated analysis walkthrough

---

## ⚙ How to Run

```bash
# 1. Clone the repository
git clone https://github.com/hariruthranhub/student-performance-result-analysis.git
cd student-performance-result-analysis

# 2. Install dependencies
pip install -r requirements.txt

# 3. Generate the dataset
python 01_generate_dataset.py

# 4. Run the full analysis (saves all 6 charts to charts/)
python 02_analysis.py

# 5. (Optional) Open the pre-run notebook
jupyter notebook Student_Performance_Analysis.ipynb
```

---

## 📓 Notebook

[`Student_Performance_Analysis.ipynb`](./Student_Performance_Analysis.ipynb)
contains the entire analysis in one narrated, pre-run walkthrough — markdown
explanations, code, and rendered chart outputs — so it's fully readable on
GitHub without needing to execute anything.

---

## 🎓 About This Project

Built by **Hari** as part of the **Naan Mudhalvan Arts Internship Program 2026**
(Python for Data Analytics track), as a hands-on project applying Python,
Pandas, NumPy, and Matplotlib to a realistic data analytics use case.

---

## 📄 License

This project is licensed under the [MIT License](./LICENSE) — free to use,
modify, and learn from.

done by Lingavel ( Naan mudhalvan arts internship python data analytics 2026)
