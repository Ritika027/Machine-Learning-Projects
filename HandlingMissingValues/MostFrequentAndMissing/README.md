# 📊 Handling Missing Categorical Data - README

## 📌 Overview

Handling missing categorical values is important for building reliable machine learning models.
Two common techniques are **Simple Imputer (constant strategy)** and **Most Frequent Imputation**.

---

## 🎯 Techniques

### 🔸 Simple Imputer (Constant)

* Replaces missing values with a **fixed constant value** (e.g., "Missing" or "Unknown")
* Useful when you want to explicitly mark missing data

---

### 🔸 Most Frequent Imputation

* Replaces missing values with the **most common category (mode)** in the column
* Helps maintain the natural distribution of data

---

## 🧠 Key Points

* Both methods prevent data loss
* Easy to implement and efficient
* Most Frequent is generally preferred for categorical features

---

## 🛠️ Example Code

Using scikit-learn:

```python
from sklearn.impute import SimpleImputer

# Constant value imputation
imputer_const = SimpleImputer(strategy='constant', fill_value='Missing')
df['Column1'] = imputer_const.fit_transform(df[['Column1']])

# Most frequent imputation
imputer_freq = SimpleImputer(strategy='most_frequent')
df['Column2'] = imputer_freq.fit_transform(df[['Column2']])
```

---

## 🚀 Conclusion

Use **constant imputation** to label missing values explicitly and **most frequent imputation** to preserve data patterns.

---
