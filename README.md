# 🚴‍♀️ Cyclistic Bike-Share Case Study (Oct 2024 – Sep 2025)

This project analyzes the **Cyclistic Bike-Share data** to uncover insights into how **casual riders** and **annual members** use the service differently.  
The analysis follows the **Google Data Analytics Capstone Case Study** framework and is fully implemented in **R Markdown** for transparency and reproducibility.

---

## 📊 Project Overview

The primary goal of this analysis is to explore user behavior patterns, time-based trends, and ride preferences to support data-driven marketing and operational strategies for Cyclistic’s growth.

### Key Questions Addressed
1. How do annual members and casual riders differ in their usage patterns?  
2. When (day, month, hour) do different types of users ride the most?  
3. What are the average ride durations and seasonal variations?  
4. What strategies could increase membership conversion?

---

## 🧩 Data Source

The dataset is derived from open-source **[Divvy Trip Data](https://divvy-tripdata.s3.amazonaws.com/index.html)** provided by **Lyft Inc.** under an open data license.  
It contains anonymized trip records from **October 2024 to September 2025** for the Chicago bike-share system.

**Data Credit:**  
Data © Lyft Inc. — Divvy Trip Data.  
All rights reserved by the original provider.

---

## 🧹 Data Cleaning and Aggregation

The original 12 monthly CSV files were cleaned and aggregated in **Excel Power Query** before being imported into R.  
The process included:

- Removing incomplete or duplicate records  
- Calculating ride duration from `started_at` and `ended_at` timestamps  
- Extracting temporal fields: **month**, **day_of_week**, and **hour**  
- Creating ride length buckets (e.g., 0–15, 15–30, 30–60 minutes)  
- Aggregating data by user type, bike type, and time intervals  

This reduced over **1 GB of raw data** into a compact **2.45 MB dataset** optimized for analysis.

---

## 🧮 Tools & Technologies

- **Excel Power Query** → Data cleaning & aggregation  
- **R (tidyverse, ggplot2)** → Data wrangling & visualization  
- **R Markdown** → Reproducible analysis report  
- **GitHub** → Version control & public sharing  

---

## 🧠 Insights Summary

- **Members** take shorter but more frequent weekday rides, aligning with commute hours (8 AM & 6 PM peaks).  
- **Casual riders** prefer longer weekend and midday rides, suggesting leisure use.  
- **Seasonal trends** show higher usage during summer months for both groups, with sharper drops for casual users.  
- **Electric bikes** are more popular among casual riders due to convenience and lower effort.

These insights can guide **marketing strategies** to encourage casual riders to become members.

---

## 📄 License

This dataset and analysis are shared under the **CC BY 4.0 License**.  
Attribution is required to both the data provider (**Lyft Inc.**) and the author (**Sameer Ahmed**).

---

## 📂 Repository Contents

| File/Folder | Description |
|--------------|-------------|
| `data/bike_ride_data.csv` | Cleaned & aggregated dataset |
| `analysis/cyclistic_case_study.Rmd` | Full R Markdown analysis file |
| `analysis/cyclistic_case_study.html` | Rendered HTML version of the analysis |
| `visuals/` | Plots and visuals used in the report |
| `README.md` | Project overview and documentation |

---

## 🧠 Author

**Sameer Ahmed**  
Data Science Enthusiast | R, Python, Power BI  
[LinkedIn](https://www.linkedin.com/in/ahmedsameer01) | [Kaggle](https://www.kaggle.com/ahmedsameer01)
