# 📊 Student Performance Dashboard (Power BI)

## 📌 Overview

The **Student Performance Dashboard** is developed using Power BI to analyze student performance, attendance, and behavior across subjects and classes.

---

## 🎯 Objectives

* Analyze student performance
* Track attendance trends
* Evaluate subject-wise scores
* Monitor behavioral patterns

---

## 📂 Data Preparation

### 🔹 Data Loading

* Dataset imported using **Get Data**

### 🔹 Data Cleaning

* Replace null values with "-"
* Corrected data types
* Processed data using **Power Query Editor**

---

## 🔗 Data Modeling

### 🔹 Relationships

* **Student Table (1)** → **Scores Table (*)** using `StudentID`
* **Student Table (1)** → **Attendance Table (*)** using `StudentID`
* **Student Table (1)** → **Behavior Table (*)** using `StudentID`

### 🔹 Configuration

* One-to-Many relationships
* Single direction filtering
* Central dimension table: **Student**

---

## 📐 DAX Measures

### 🔹 1. Percentage Score

```DAX
% Score = 
DIVIDE(SUM(Scores[Score]), SUM(Scores[MaxScore]), 0)
```

### 🔹 2. Average Score Per Subject

```DAX
Avg Score Per Subject = 
AVERAGE(Scores[Score])
```

### 🔹 3. Attendance Percentage

```DAX
Attendance % = 
DIVIDE(
    CALCULATE(COUNT(Attendance[Status]), Attendance[Status] = "Present"),
    COUNT(Attendance[Status]),
    0
)
```

### 🔹 4. Behavior Count

```DAX
Behavior Count = 
COUNT(Behavior[BehaviorType])
```

### 🔹 5. Performance Category

```DAX
Performance Category = 
SWITCH(
    TRUE(),
    [% Score] >= 0.8, "High",
    [% Score] >= 0.4, "Medium",
    "Low"
)
```

---

## 📊 Dashboard Features

* Dashboard have two pages one was Executive dashboard and second was drillthrow student page
* KPI Cards for key metrics
* Subject-wise performance charts
* Attendance trend analysis
* Behavior distribution visualization

---

## 🚀 Conclusion

This dashboard provides meaningful insights into student performance using Power BI with effective data modeling and DAX calculations.

---
