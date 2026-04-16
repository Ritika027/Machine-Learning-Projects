# 🔢 Ordinal Encoding in Machine Learning

## 📌 Overview

Ordinal Encoding is a technique used to convert **categorical data with an inherent order** into numerical values. Each category is assigned a unique integer based on its ranking or order.

---

## 🎯 Why Ordinal Encoding is Important

* Preserves the **order or ranking** of categories
* Helps ML models understand **relative importance**
* Simple and memory-efficient compared to One-Hot Encoding
* Useful when categories have meaningful progression

---

## ⚙️ How Ordinal Encoding Works

Each category is assigned a number based on its order.

### 🧾 Example

| Size   | Encoded Value |
| ------ | ------------- |
| Small  | 0             |
| Medium | 1             |
| Large  | 2             |

---

## 🧪 Example in Python (Using Pandas)

```python id="k2d8fa"
import pandas as pd

# Sample data
data = {'Size': ['Small', 'Medium', 'Large', 'Medium']}
df = pd.DataFrame(data)

# Define order
order = {'Small': 0, 'Medium': 1, 'Large': 2}

# Apply encoding
df['Size_encoded'] = df['Size'].map(order)

print(df)
```

---

## 🔧 Using Scikit-learn

```python id="s7m1pd"
from sklearn.preprocessing import OrdinalEncoder
import numpy as np

# Sample data
data = np.array([['Small'], ['Medium'], ['Large']])

encoder = OrdinalEncoder(categories=[['Small', 'Medium', 'Large']])
encoded = encoder.fit_transform(data)

print(encoded)
```

---

## 📊 When to Use Ordinal Encoding

* When data has **natural order**, such as:

  * Education level (High School < Bachelor < Master)
  * Ratings (Low < Medium < High)
  * Sizes (Small < Medium < Large)

---

## ⚠️ Limitations

* Assumes equal spacing between categories (which may not be true)
* Can mislead models if order is not meaningful
* Not suitable for nominal data (use One-Hot instead)

---

## 🔄 Comparison with Other Encoding

| Encoding Type    | Order Preserved | Columns Created |
| ---------------- | --------------- | --------------- |
| Ordinal Encoding | ✅ Yes           | 1               |
| One-Hot Encoding | ❌ No            | Multiple        |

---

## 📌 Conclusion

Ordinal Encoding is an efficient way to convert ordered categorical data into numerical form while preserving its hierarchy. It is best suited for features where ranking plays an important role in prediction.

---

## 🔗 Author

Created as part of Machine Learning tutorial practice.
