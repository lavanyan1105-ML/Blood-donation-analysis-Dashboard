# 🩸 Blood Donation Analysis using Power BI & Data Warehousing

## 📌 Overview

The availability of blood donors is essential for saving lives. However, factors such as personal health, lifestyle habits, and misconceptions often reduce participation.

This project analyzes health and wellness survey data to understand donor behavior and identify ways to improve blood donation participation.

---

## 🎯 Objectives

* Analyze factors affecting blood donation willingness
* Identify barriers and misconceptions
* Discover potential donor groups
* Provide actionable recommendations

---

## 🛠️ Tools & Technologies

* **Power BI** – Data Visualization
* **Google Forms** – Data Collection
* **Google Sheets** – Data Cleaning & Storage
* **SQL** – Data Warehousing & Querying

---

## 📊 Dataset Information

* **Dataset Name:** Health and Wellness Profile Survey
* **Source:** Self-collected survey
* **Size:** 100+ responses
* **Attributes:**

  * Age, Gender
  * Blood Group
  * Height, Weight (BMI)
  * Lifestyle Habits (Diet, Sleep, Exercise)
  * Substance Use
  * Willingness to Donate
  * Past Donation History

---

## 📈 Data Visualization

Visualizations created using Power BI:

* 📊 Bar Charts – Blood group distribution
* 📉 Scatter Plots – Height vs Weight vs Willingness
* 🔥 Heatmaps – Lifestyle vs Donation Willingness

---

## 🔍 Key Insights

### 👥 Demographics

* Majority: Age 18–25 (students)
* Most common blood groups: O+ and B+

### ❤️ Willingness to Donate

* ~60% willing to donate
* Unwilling due to fear, health concerns, and lack of awareness

### 🏃 Lifestyle Impact

* Exercise & good sleep → Higher willingness
* Smoking & alcohol → Lower willingness

### 🚫 Barriers

* Fear of needles
* Misconceptions about eligibility
* Lack of awareness

---

## 🏗️ Data Warehousing

### Schema

* Snowflake Schema
* Fact Table: Donation data
* Dimension Tables:

  * Demographics
  * Blood Group
  * Lifestyle

---

## 🔄 ETL Process

1. **Extraction:** Google Forms → CSV
2. **Transformation:** Data cleaning, standardization, categorization
3. **Loading:** SQL database with indexing

---

## 🧠 Sample SQL Queries

```sql
SELECT BloodGroup, COUNT(*) 
FROM Participants 
WHERE WillingToDonate = 'Yes' 
GROUP BY BloodGroup;
```

```sql
SELECT AVG(SleepHours) 
FROM Participants 
WHERE WillingToDonate = 'Yes';
```

---

## ⚡ Performance

* Indexed key columns (BloodGroup, WillingToDonate)
* Query execution time < 1 second

---

## 📌 Results

* Identified awareness gaps in blood donation
* Found strong potential donor group (students)
* Highlighted importance of targeting rare blood groups

---

## ✅ Conclusion

Health, lifestyle, and awareness significantly influence blood donation behavior.

Improving education and addressing misconceptions can:

* Increase donor participation
* Build a strong donor network
* Support emergency healthcare needs

---

## 📂 Project Structure

```
blood-donation-analysis/
│
├── data/
├── powerbi/
├── sql/
├── docs/
└── README.md
```

---

## 📚 References

* Health and Wellness Survey Dataset
* Research on blood donation trends
* Power BI Documentation

---

## 👩‍💻 Author

**Lavanya**
Final Year CSE (Data Science)
