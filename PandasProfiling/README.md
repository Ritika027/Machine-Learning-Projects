# 📊 Pandas Profiling (ydata-profiling) 

## 📌 Overview

This project demonstrates how to perform **Exploratory Data Analysis (EDA)** using **Pandas Profiling** (now known as **ydata-profiling**) in Python.
It helps in generating a **complete automated report** of a dataset with just a few lines of code.

---

## 🚀 What is Pandas Profiling?

Pandas Profiling ek powerful Python library hai jo dataset ka **detailed analysis report** automatically generate karta hai.
Isme aapko milta hai:

* Dataset summary
* Missing values analysis
* Correlation between features
* Distribution of each column
* Outliers detection
* Data types and uniqueness

---

## 🛠️ Installation

```bash
pip install ydata-profiling
```

---

## 📂 Project Structure

```
├── data/
│   └── dataset.csv
├── pandas_profiling.ipynb
├── report.html
└── README.md
```

---

## ⚙️ Usage

### Step 1: Import Libraries

```python
import pandas as pd
from ydata_profiling import ProfileReport
```

### Step 2: Load Dataset

```python
df = pd.read_csv("dataset.csv")
```

### Step 3: Generate Report

```python
profile = ProfileReport(df, explorative=True)
profile.to_file("report.html")
```

---

## 📊 Features Explained (Hinglish)

### 1. Overview

Dataset ka basic info jaise:

* Total rows & columns
* Memory usage
* Duplicate rows

### 2. Variables Section

Har column ka detail:

* Mean, Median, Mode
* Unique values
* Missing values

### 3. Correlation

Features ke beech relation:

* Pearson correlation
* Spearman correlation

### 4. Missing Values

Kaunsa column me kitna missing data hai (visual format me)

### 5. Sample Data

Top and bottom rows preview

---

## 🎯 Use Cases

* Data preprocessing se pehle quick understanding
* Machine Learning projects me EDA
* Data cleaning decisions lene ke liye
* Feature selection ke liye

---

## ✅ Advantages

* Time saving (manual EDA ki zarurat kam)
* Beginner-friendly
* Visual and interactive report
* One-line analysis

---

## ⚠️ Limitations

* Large datasets me slow ho sakta hai
* High memory consumption
* Custom analysis limited hota hai

---

## 📌 Conclusion

Pandas Profiling ek **fast aur efficient tool** hai jo data analysis ko easy bana deta hai.
Agar aap beginner ho ya quick EDA karna chahte ho, toh yeh best tool hai.

---

