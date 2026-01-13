# 🌍 Air Quality & Air Pollution Data Analysis Project

## 📌 Project Overview
This project focuses on **data cleaning, exploratory data analysis (EDA), and insights generation**
from an air quality and air pollution dataset. The goal is to convert raw, incomplete data into a
**clean, analysis-ready dataset** and derive meaningful insights.

This project demonstrates practical **Data Analyst skills** such as data preprocessing,
handling missing values, and domain-driven decision making.

---

## 🎯 Objectives
- Clean and preprocess air pollution data
- Handle missing values using statistical and rule-based methods
- Perform exploratory data analysis (EDA)
- Analyze air quality patterns across cities
- Prepare a final cleaned dataset for analysis or modeling

---

## 🗂️ Dataset Description
The dataset includes air quality measurements from multiple cities with the following features:

- City  
- Date  
- PM2.5, PM10  
- NO, NO2, NOx  
- NH3, CO, SO2, O3  
- Benzene, Toluene, Xylene  
- AQI (Air Quality Index)  
- AQI_Bucket (Air Quality Category)

---

## 🧹 Data Cleaning Process

### 1. Missing Value Analysis
- Calculated missing value counts and percentages
- Identified columns with high missing values (PM10, NH3, AQI_Bucket)

### 2. Numerical Feature Imputation
- Applied **city-wise median imputation** to preserve local pollution patterns
- Used **global median fallback** when city-level data was completely missing

### 3. AQI_Bucket Handling (Categorical)
- Avoided statistical imputation
- Used **rule-based classification** based on AQI values
- AQI categories assigned using CPCB standards:
  - 0–50 → Good
  - 51–100 → Moderate
  - 101–200 → Satisfactory
  - 201–300 → Poor
  - 301–400 → Very Poor
  - >400 → Severe

### 4. Data Validation
- Verified missing values after cleaning
- Ensured consistency between AQI and AQI_Bucket

---

## 📊 Exploratory Data Analysis (EDA)
- Distribution analysis of pollutant levels
- Identification of skewed features
- AQI comparison across different cities
- Pattern recognition in air pollution data

---

## 🛠️ Tools & Technologies Used
- Python
- Pandas
- NumPy
- Matplotlib / Seaborn
- Jupyter Notebook
- Git & GitHub

---

## 📌 Key Learnings
- Real-world datasets require multi-level missing value strategies
- Domain knowledge is crucial for categorical feature handling
- City-wise grouping improves imputation accuracy
- Clean data leads to reliable insights

---

## 🚀 How to Use This Project
1. Clone the repository
2. Open the Jupyter Notebook
3. Run all cells sequentially
4. Explore EDA results and cleaned dataset

---

## 👤 Author
**Sanjai CR**  
Aspiring Data Analyst  
Skills: Python | SQL | Machine Learning | Power BI | Tableau | Excel | AI

---

## ⭐ If you like this project
Please ⭐ the repository and feel free to connect!
