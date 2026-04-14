# 📊 Normalization (Min-Max Scaling) – README

## 📌 Overview

This project demonstrates how to apply **Normalization** (also known as **Min-Max Scaling**) on a dataset using Python.
Normalization ek important preprocessing technique hai jo data ko **fixed range (usually 0 to 1)** me convert karta hai.

---

## 🎯 Objectives

* Feature scaling ka concept samajhna
* Normalization apply karna dataset par
* Before vs After comparison dekhna
* Machine Learning models ke liye data prepare karna

---

## 🚀 What is Normalization?

Normalization ek technique hai jisme data ko rescale kiya jata hai so that saare values ek **specific range (0 to 1)** ke andar aa jayein.

👉 Formula:
x' = (x - min) / (max - min)

Where:

* x = original value
* min = minimum value of feature
* max = maximum value of feature

---

## 📂 Project Structure

```
├── dataset.csv
├── normalization.ipynb
├── normalized_data.csv
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
from sklearn.preprocessing import MinMaxScaler
```

### Step 2: Load Dataset

```python
df = pd.read_csv("dataset.csv")
```

### Step 3: Apply Normalization

```python
scaler = MinMaxScaler()
normalized_data = scaler.fit_transform(df)

df_normalized = pd.DataFrame(normalized_data, columns=df.columns)
```

---

## 📊 Features Explained (Hinglish)

### 🔹 Fixed Range (0 to 1)

Saare values 0 aur 1 ke beech aa jaate hain

### 🔹 Shape Preservation

Data ka original distribution shape mostly same rehta hai

### 🔹 Sensitive to Outliers

Agar outliers ho, toh scaling distort ho sakti hai

---

## 📈 When to Use Normalization?

* Jab data ka distribution known nahi ho
* Algorithms like:

  * KNN
  * Neural Networks
  * Gradient Descent based models

---

## ✅ Advantages

* Data ko uniform scale me laata hai
* Distance-based algorithms ke liye useful
* Easy to understand and implement

---

## ⚠️ Limitations

* Outliers ka strong effect hota hai
* New data aane par re-scaling required hoti hai
* Standardization jitna robust nahi hota

---

## 📌 Conclusion

Normalization ek **simple aur effective scaling technique** hai jo especially distance-based models ke liye useful hoti hai.
Agar aapko data ko fixed range me lana hai, toh Normalization best choice hai.

---

