# 📊 Categorical Data Analysis using Python

---

## 🧾 Experiment Title

**Study of Categorical Data Analysis using Python**

---

## 🎯 Aim

To understand and perform analysis on categorical data using Python libraries like **Pandas** and **Matplotlib**.

---

## 📚 Theory

Categorical data represents data that can be divided into groups or categories. These categories are usually **non-numeric** and represent labels or names.

### 🔹 Types of Categorical Data:

* **Nominal Data** 🏷️
  No specific order (e.g., gender, color, city)

* **Ordinal Data** 📈
  Has a meaningful order (e.g., grades, ratings)

---

## 🛠️ Tools & Libraries Used

* 🐍 Python
* 📦 Pandas
* 📊 Matplotlib / Seaborn

---

## 💻 Code Implementation

### 🔸 1. Import Libraries

```python
import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns
```

---

### 🔸 2. Create Sample Dataset

```python
data = {
    'Name': ['A', 'B', 'C', 'D', 'E'],
    'Gender': ['Female', 'Male', 'Female', 'Male', 'Female'],
    'Department': ['IT', 'HR', 'IT', 'Finance', 'HR']
}

df = pd.DataFrame(data)
print(df)
```

---

### 🔸 3. Count Frequency of Categories

```python
print(df['Gender'].value_counts())
print(df['Department'].value_counts())
```

---

### 🔸 4. Convert to Categorical Type

```python
df['Gender'] = df['Gender'].astype('category')
print(df.dtypes)
```

---

### 🔸 5. Visualization (Bar Chart)

```python
df['Department'].value_counts().plot(kind='bar')
plt.title("Department Distribution")
plt.xlabel("Department")
plt.ylabel("Count")
plt.show()
```

---

### 🔸 6. Using Seaborn Count Plot

```python
sns.countplot(x='Gender', data=df)
plt.title("Gender Count")
plt.show()
```

---

## 📊 Observations

* Categorical data helps in understanding patterns and distributions.
* Frequency counts are useful to summarize categories.
* Visualization makes analysis easy and clear.

---

## ✅ Conclusion

Categorical data analysis is essential for understanding grouped data. Using Python libraries like Pandas and visualization tools, we can easily analyze and interpret such data efficiently.

---

## 💡 Applications

* 📈 Market Research
* 🧑‍🤝‍🧑 Customer Segmentation
* 🏥 Healthcare Analysis
* 🛒 Sales & Business Insights

---

## 🚀 Extra Tip

Use `.value_counts(normalize=True)` to get percentage distribution instead of counts 😉

---

✨ *Happy Coding!* ✨
