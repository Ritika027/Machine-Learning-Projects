# 📊 Standardization (Z-Score Normalization) – README

## 📌 Overview

This project demonstrates how to apply **Standardization** (also called **Z-score normalization**) on a dataset using Python.
Standardization ek important preprocessing step hai jo data ko **mean = 0** aur **standard deviation = 1** ke scale par convert karta hai.

---

## 🎯 Objectives

* Feature scaling ka concept samajhna
* Standardization apply karna dataset par
* Before vs After comparison dekhna
* Machine Learning models ke liye data prepare karna

---

## 🚀 What is Standardization?

Standardization ek technique hai jisme har data point ko uske mean aur standard deviation ke respect me scale kiya jata hai.

👉 Formula:
z = (x - μ) / σ

Where:

* x = original value
* μ = mean of feature
* σ = standard deviation

---

## 📂 Project Structure

```
├── dataset.csv
├── standardization.ipynb
├── standardized_data.csv
└── README.md
```

---

## 🛠️ Installation

```bash
pip install pandas numpy scikit-learn
```

---

## ⚙️ Usage

### Step 1: Import Libraries

```python
import pandas as pd
from sklearn.preprocessing import StandardScaler
```

### Step 2: Load Dataset

```python
df = pd.read_csv("dataset.csv")
```

### Step 3: Apply Standardization

```python
scaler = StandardScaler()
scaled_data = scaler.fit_transform(df)

df_scaled = pd.DataFrame(scaled_data, columns=df.columns)
```

---

## 📊 Features Explained (Hinglish)

### 🔹 Mean Centering

Data ka mean 0 ho jata hai (center shift ho jata hai)

### 🔹 Unit Variance

Standard deviation 1 ho jata hai → sab features same scale pe aa jate hain

### 🔹 No Fixed Range

Normalization ke unlike, yeh data ko 0–1 range me nahi laata

---

## 📈 When to Use Standardization?

* Jab data normally distributed ho
* Algorithms like:

  * Linear Regression
  * Logistic Regression
  * KNN
  * SVM

---

## ✅ Advantages

* Model performance improve karta hai
* Gradient descent fast converge karta hai
* Outliers ke effect ko thoda control karta hai

---

## ⚠️ Limitations

* Outliers still impact kar sakte hain
* Interpretation thoda difficult ho jata hai
* Original units lost ho jate hain

---

## 📌 Conclusion

Standardization ek **powerful preprocessing technique** hai jo Machine Learning models ko efficient banati hai.
Agar aapka data different scales me hai, toh Standardization use karna highly recommended hai.

---


