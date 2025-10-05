# 📊 Waze User Churn Analysis  

## 📌 Project Overview  
This project analyzes user churn in Waze’s driver dataset. The goal is to investigate behavioral patterns that differentiate **churned** vs. **retained** users and provide actionable insights to improve retention strategies.  


---

## 🎯 Objectives  
- Inspect and prepare Waze driver data for analysis  
- Identify missing values, inconsistencies, and data types  
- Compare behavioral patterns between churned and retained users  
- Explore potential churn drivers such as trip frequency, distance, and device type  
- Summarize findings in an executive-style report for the data team  

---

## 🛠️ Tools & Libraries  
- **Python**  
- **Pandas** (data cleaning & manipulation)  
- **NumPy** (statistical calculations)  

---

## 📂 Dataset  
- **Source:** Provided Waze dataset (~15,000 users)  
- **Key variables:**  
  - `label`: User retention status (retained or churned)  
  - `drives`: Number of drives last month  
  - `driving_days`: Days app was used  
  - `driven_km_drives`: Distance driven (km)  
  - `device`: Device type (iPhone / Android)  

---

## 🔎 Analysis Process  
1. **Data Inspection** – Checked structure, missing values, and data types  
2. **Missing Data Analysis** – Found ~700 missing values in the `label` column; distribution was random across devices  
3. **Exploratory Analysis** – Compared churned vs. retained user behaviors (distance, drives, usage days)  
   - Created derived metrics (e.g., `km_per_drive`, `drives_per_driving_day`)  
   - Analyzed device type distribution (iPhone vs. Android)  
4. **Summary Statistics** – Used medians to avoid skew from outliers  

---

## 📈 Key Findings  
- **Churned users**: Drove longer distances and more hours, but on fewer days → suggesting “super-drivers”  
- **Retained users**: Used the app more consistently across the month  
- **Device type**: iPhone (~64%) vs. Android (~36%) split; churn rates were similar across devices  
- **Missing labels**: Randomly distributed, no evidence of bias  

---

## 📝 Executive Insights  
- Users who churn tend to drive **farther and longer in fewer sessions** compared to retained users  
- Retained users are more engaged with the app on a **day-to-day basis**  
- Churn is **not strongly correlated with device type**  
- Recommended further study on **super-drivers** to understand why Waze may not meet their needs  

---

## 📚 Skills Demonstrated  
- Data Cleaning & Preparation  
- Exploratory Data Analysis (EDA)  
- Statistical Analysis (median vs. mean)  
- Churn Analysis & Business Insights  

---
