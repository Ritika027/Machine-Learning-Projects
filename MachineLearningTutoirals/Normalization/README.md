# 📊 Normalization in Machine Learning

## 📌 Overview

Normalization is a data preprocessing technique used in Machine Learning to scale numerical features into a common range, usually between **0 and 1**. It helps improve model performance and ensures that no feature dominates others due to its scale.

---

## 🎯 Why Normalization is Important

* Ensures all features contribute equally to the model
* Improves convergence speed of algorithms
* Prevents bias due to large-value features
* Essential for distance-based algorithms like KNN and clustering

---

## ⚙️ Types of Normalization

### 1. Min-Max Normalization

Scales values between 0 and 1.

**Formula:**

```
X_norm = (X - X_min) / (X_max - X_min)
```

---

### 2. Mean Normalization

Centers data around mean.

**Formula:**

```
X_norm = (X - Mean) / (X_max - X_min)
```

---

### 3. Max Normalization

Scales values by dividing with maximum value.

**Formula:**

```
X_norm = X / X_max
```

---

## 🧪 Example in Python

```python
from sklearn.preprocessing import MinMaxScaler
import pandas as pd

# Sample data
data = {'Age': [18, 22, 25, 30, 35]}
df = pd.DataFrame(data)

# Apply normalization
scaler = MinMaxScaler()
df['Age_normalized'] = scaler.fit_transform(df[['Age']])

print(df)
```

---

## 📊 When to Use Normalization

* When features have different scales
* In algorithms like:

  * K-Nearest Neighbors (KNN)
  * Neural Networks
  * Gradient Descent-based models

---

## 🚫 When NOT to Use

* Tree-based models (Decision Tree, Random Forest) usually don’t require normalization

---

## 📌 Conclusion

Normalization is a simple but powerful preprocessing step that ensures better performance and stability of Machine Learning models by bringing all features to the same scale.

---

## 🔗 Author

Created as part of Machine Learning tutorial practice.
