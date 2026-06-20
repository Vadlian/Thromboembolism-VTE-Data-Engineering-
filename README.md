# Thromboembolism-VTE-Data-Engineering-
A data engineering and data cleansing project using Python and Pandas to process, validate, and analyze messy Venous Thromboembolism (VTE) hospital admission datasets.
# Healthcare Data Engineering & Quality Analytics (Python & Pandas)

## 📌 Project Overview
This project focuses on the end-to-end data engineering, structural cleansing, and quality validation of a messy, multi-column clinical NHS dataset tracking Venous Thromboembolism (VTE) hospital admissions. The goal was to take raw, improperly formatted data and transform it into a reliable, analytical-ready asset for healthcare reporting.

## 🛠️ Tech Stack & Tools
* **Language:** Python
* **Libraries:** Pandas, NumPy, Matplotlib, Seaborn
* **Environment:** Jupyter Notebook

## 🚀 Key Data Challenges Solved
* **Data Ingestion & Structural Cleanse:** Managed custom semi-colon delimiters and implemented programmatic stripping to fix alignment bugs caused by leading and trailing whitespace in the column headers.
* **Relative Position Tracking:** Bypassed duplicate text header column traps by utilizing `.iloc` relative position tracking to maintain exact data alignment.
* **Data Type Coercion:** Handled non-numeric string gaps and text placeholders, programmatically converting them into clean, operational numeric values using `pd.to_numeric`.
* **Statistical Integrity & Boundary Clipping:** Identified human-reporting entry anomalies where screening metrics mathematically exceeded 100% capacity. Engineered data-validation logic implementing boundary clipping via `np.clip` to enforce realistic aggregate reporting thresholds.
* **Exploratory Data Analysis (EDA):** Leveraged advanced `.groupby()` aggregations to isolate regional variations and performance metrics across different health sectors.

## 📊 Visualizations & Results
The final phase of the pipeline generates warning-free, presentation-ready dashboard charts using Seaborn to visualize geographical patient distribution and regional health sector volumes, ensuring medical administrators have clear, executive-level insights.

---
*Note: This project forms part of my foundational portfolio prep ahead of entering my Diploma in Health Records & Information Technology.*
