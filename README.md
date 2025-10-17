# 🌍 Air Quality and Air Pollution Analysis

## 📘 Overview
This project focuses on analyzing **air quality and pollution levels** across multiple Indian cities to understand key pollutants, seasonal variations, and overall air quality trends.  
Using **Python-based data analytics**, the goal is to derive actionable insights that can support environmental monitoring and public health awareness.

---

## 🎯 Objectives
- Clean and preprocess large-scale air quality datasets.
- Analyze pollutant levels and Air Quality Index (AQI) trends.
- Identify the most affected cities and potential causes.
- Visualize pollution distribution and seasonal patterns.

---

## 🧰 Tools & Technologies
- **Programming Language:** Python  
- **Libraries Used:** Pandas, NumPy, Matplotlib  
- **Environment:** Jupyter Notebook  
- **Dataset:** City Day Air Quality Dataset (India)

---

## 🧹 Data Cleaning & Preprocessing
- Loaded the dataset using **Pandas**.
- Removed **duplicates** and handled **missing values**.
- Filled missing pollutant values using **median imputation** (city-wise approach).
- Converted the `Date` column into **datetime format** and extracted:
  - `Year`
  - `Month`
  - `Day`
- Ensured data consistency and completeness for analysis.

---

## 📊 Exploratory Data Analysis (EDA)
### Key Analysis Steps
- Examined the distribution of pollutants such as:
  - **PM2.5**, **PM10**, **NO**, **NO2**, **NOx**, **NH3**, **CO**, **SO2**, **O3**, and **AQI**.
- Plotted **histograms** to understand pollution concentration levels.
- Analyzed **city-wise averages** of key pollutants.
- Explored **AQI buckets** to identify the proportion of "Good", "Moderate", and "Poor" air quality days.
- Observed **time-based variations** in pollution levels.

---

## 📈 Visualizations
- **Distribution Graphs:** Showed frequency of pollutant levels.
- **City-wise Bar Charts:** Compared average pollutant concentrations across cities.
- **AQI Trend Analysis:** Displayed changes in air quality over time.

Sample Visualization:
```python
df.groupby("City")[['PM2.5','PM10','NO2','O3']].mean().plot(kind='bar', figsize=(12,6))
plt.title('Average Pollution Level per City')
plt.xlabel('City')
plt.ylabel('Average Pollutant Level')
plt.grid()
plt.show()
