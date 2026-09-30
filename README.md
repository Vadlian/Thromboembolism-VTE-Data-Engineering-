# 🩺 Healthcare Data Engineering & Quality Analytics (Python & Pandas)

[![Python](https://img.shields.io/badge/Python-3.9+-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org/)
[![Pandas](https://img.shields.io/badge/Pandas-1.5+-150458?style=for-the-badge&logo=pandas&logoColor=white)](https://pandas.pydata.org/)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626?style=for-the-badge&logo=jupyter&logoColor=white)](https://jupyter.org/)

A data engineering and data cleansing pipeline designed to process, validate, and analyze messy Venous Thromboembolism (VTE) hospital admission datasets.

---

## 📌 Project Overview
This project focuses on the end-to-end data engineering, structural cleansing, and quality validation of a messy, multi-column clinical NHS dataset tracking **Venous Thromboembolism (VTE)** hospital admissions. 

The primary goal was to take raw, improperly formatted clinical data and transform it into a reliable, analytics-ready data asset suitable for executive reporting and medical administrators.

---

## 🛠️ Tech Stack & Tools
* **Language:** Python
* **Data Processing & Engineering:** Pandas, NumPy
* **Data Visualization:** Matplotlib, Seaborn
* **Environment:** Jupyter Notebook / Python Scripts

---

## 🚀 Key Data Engineering Challenges Solved

### 1. Data Ingestion & Structural Cleanse
Handled custom semi-colon delimiters and implemented programmatic string manipulation (`.str.strip()`) to resolve alignment bugs caused by erratic leading and trailing whitespace in column headers.

### 2. Relative Position Tracking
Bypassed duplicate text header column traps by utilizing **`.iloc` relative position tracking** to maintain strict positional data alignment across inconsistent sheets.

### 3. Data Type Coercion
Identified non-numeric string gaps and text placeholders, programmatically coercing them into clean, operational numeric formats using `pd.to_numeric(..., errors='coerce')`.

### 4. Statistical Integrity & Boundary Clipping
Identified human-reporting entry anomalies where screening metrics mathematically exceeded 100% capacity. Engineered data-validation logic implementing boundary clipping via `np.clip` to enforce realistic aggregate reporting thresholds (0–100%).

### 5. Exploratory Data Analysis (EDA)
Leveraged advanced `.groupby()` aggregations and pivot operations to isolate regional variations and evaluate performance metrics across different health sectors.

---

## 📊 Visualizations & Outputs
The final phase of the pipeline generates warning-free, presentation-ready dashboard charts using **Seaborn** to visualize:
* Geographical patient distribution across regions.
* Regional health sector throughput and compliance volumes.

These outputs ensure healthcare decision-makers receive clear, actionable insights derived from verified, clean data.

---

> **Note:** This project forms part of my core technical portfolio ahead of my Diploma in Information Technology studies.

