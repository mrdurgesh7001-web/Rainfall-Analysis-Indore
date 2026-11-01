# 🌧️ Rainfall Analysis (2001–2026) | Madhya Pradesh, India

## 📌 Project Overview

This project focuses on analyzing daily rainfall data from 2001 to 2026 to understand rainfall patterns, seasonal distribution, year-to-year variations, and long-term monsoon trends.

Using Python, Pandas, NumPy, Matplotlib, and Seaborn, I explored how rainfall changes over time, how it is distributed across months, and how frequently dry periods occur.

The main objective is to go beyond simply measuring total rainfall and understand **how much it rains, when it rains, and how rainfall patterns vary over time.**

## 🎯 Project Objectives

- Analyze daily and annual rainfall patterns.
- Understand monthly and seasonal rainfall distribution.
- Identify rainy days and dry days.
- Classify rainfall into different intensity categories.
- Analyze consecutive dry spells.
- Compare June–September monsoon rainfall across years.
- Calculate rainfall deviations from the historical dataset average.
- Examine long-term rainfall trends using statistical methods.

## 📂 Dataset Information

**Dataset:** `rainfalldata_2001_to_2026.csv`

| Attribute | Description |
|---|---|
| YEAR | Year of observation |
| DOY | Day of the year |
| PRECTOTCORR | Corrected precipitation (mm/day) |

- **Time period:** 2001–2026
- **Total records:** 9,422 daily observations
- **2001–2025:** Complete calendar-year records
- **2026:** Partial-year records, available through Day 291

The dataset contains daily precipitation values. Additional features such as Date, Month, Day_Name, Rainy_Day, and Rain_Type are created during analysis.

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- PyMannKendall
- Jupyter Notebook

## 🔍 Analysis Performed

### 1. Data Validation and Preparation
- Checked dataset dimensions, data types, and descriptive statistics.
- Checked missing values and duplicate records.
- Validated year and day-of-year values.
- Created date-related columns for time-based analysis.

### 2. Rainfall Classification

Rainfall observations were classified into intensity categories:

| Rainfall (mm/day) | Category |
|---|---|
| 0 mm | No precipitation recorded |
| 0.1–2.4 mm | Very Light |
| 2.5–15.5 mm | Light |
| 15.6–64.4 mm | Moderate |
| 64.5–115.5 mm | Heavy |
| 115.6–204.4 mm | Very Heavy |
| 204.5 mm or more | Extremely Heavy |

### 3. Rainy Days and Dry Days
- Compared the frequency of rainy and dry days.
- Analyzed the distribution of rainfall intensity categories.
- Examined how rainfall intensity varies across years.

### 4. Monthly and Annual Rainfall Analysis
- Calculated total rainfall year-wise.
- Analyzed monthly rainfall distribution.
- Created a year-versus-month rainfall heatmap.
- Compared rainfall contributions from different months.

### 5. Dry Spell Analysis
- Identified consecutive days with zero recorded precipitation.
- Calculated the longest dry spell for each year.
- Identified and compared the top 10 longest dry spells.

### 6. Southwest Monsoon Analysis

Focused on the main monsoon period:

**June, July, August, and September.**

The analysis includes:
- Year-wise monsoon rainfall.
- Average monsoon rainfall across the analyzed years.
- Above-average and below-average years.
- Percentage deviation from the dataset's historical average.
- Year-to-year rainfall changes.

### 7. Rainfall Trend Analysis
- Visualized long-term monsoon rainfall trends.
- Applied linear regression to estimate the yearly trend.
- Used the Mann–Kendall statistical test to examine whether a monotonic trend exists.

## 📊 Key Findings

The analysis produced several observations:

- Approximately **91.43%** of the recorded rainfall in the dataset occurred during June–September.
- The linear trend analysis estimated an increase of approximately **13.02 mm/year** in monsoon rainfall.
- The Mann–Kendall test indicated an increasing trend, with a p-value of approximately **0.03** and an estimated Sen's slope of **13.53 mm/year**.
- Rainfall varied considerably between years, with both above-average and below-average monsoon seasons.
- Dry spells and rainfall intensity provided additional information beyond total rainfall.

*Note: These are dataset-derived results, not official IMD rainfall classifications or forecasts. Statistical trend results should be interpreted with the test assumptions and dataset limitations in mind.*

## 📈 Visualizations

The notebook includes:

- Rainy Days vs Dry Days
- Rainfall Intensity Distribution
- Year-wise Total Rainfall
- Monthly Rainfall Distribution
- Year-wise Monthly Rainfall Heatmap
- Longest Consecutive Dry Spells
- Top 10 Longest Dry Spells
- Year-wise Monsoon Rainfall
- Above-average vs Below-average Monsoon Years
- Monsoon Rainfall Deviation
- Long-term Rainfall Trend
- Year-to-Year Rainfall Changes

## ⚠️ Limitations

- The dataset represents a selected geographical location or data point, not every district of Madhya Pradesh.
- Gridded or model-derived precipitation data may differ from local rain-gauge observations.
- The 2026 data is incomplete for the calendar year and should not be treated as a full-year total.
- The historical average calculated in this project is a dataset-based reference, not necessarily the official IMD climatological normal.
- Rainfall alone cannot determine groundwater availability, agricultural water availability, or drought conditions.

## 🚀 Future Scope

Possible improvements include:

- Comparing rainfall data with official IMD observations.
- Extending the analysis to multiple locations and districts.
- Studying rainfall variability and extreme rainfall events.
- Combining rainfall data with groundwater and reservoir information.
- Developing an interactive rainfall analysis dashboard.

## 💡 What I Learned

Through this project, I practiced:

- Working with time-series data.
- Data validation and feature engineering.
- GroupBy, Pivot Tables, and aggregation in Pandas.
- Exploratory Data Analysis (EDA).
- Data visualization using Matplotlib and Seaborn.
- Identifying dry spells and seasonal patterns.
- Applying statistical methods to analyze trends.
- Interpreting data-driven findings and their limitations.

## 📁 Repository Structure

```text
Rainfall-Analysis/
│
├── rainfalldata_2001_to_2026.csv
├── rainfalldata_2001_to_2026.ipynb
└── README.md
```

## 👨‍💻 Author

**Durgesh Choudhary**

BSc Data Science Student

Interested in Data Science, Data Analytics, Python, and Machine Learning.

---

*This project is an exploratory data analysis project focused on understanding historical rainfall patterns and monsoon variability.*
