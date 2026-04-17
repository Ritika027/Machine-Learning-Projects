# 📊 Filling Missing Values using Mean & Median - README

## 📌 Overview

Handling missing data is an important step in data preprocessing.
Two common techniques are **Mean Imputation** and **Median Imputation**, where missing values are replaced with a central value of the column.

---

## 🎯 Mean Imputation

* Replace missing values with the **average (mean)** of the column
* Works well when data is **normally distributed (no extreme outliers)**

👉 Formula:
Mean = Sum of values / Number of values

---

## 🎯 Median Imputation

* Replace missing values with the **middle value (median)**
* Works well when data has **outliers or skewed distribution**

👉 Median = Middle value after sorting data

---

## ⚖️ Mean vs Median

| Method | Best For            | Sensitive to Outliers |
| ------ | ------------------- | --------------------- |
| Mean   | Normal distribution | Yes ❌                 |
| Median | Skewed data         | No ✅                  |

---

## 🧠 Key Points

* Both methods are simple and fast
* They prevent data loss (unlike dropping rows)
* Median is generally more robust than mean

---

## 🚀 Conclusion

Use **mean imputation** for clean, symmetric data and **median imputation** when data contains outliers or is skewed.

---
