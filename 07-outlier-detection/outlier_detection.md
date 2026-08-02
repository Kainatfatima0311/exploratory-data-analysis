# Outlier Detection

## Definition

An outlier is a value that is significantly different from the rest of the observations in a dataset.

---

## Why Detect Outliers?

- Improve data quality
- Prevent misleading statistics
- Improve machine learning models

---

## Detect Using Box Plot

```python
sns.boxplot(x=df["Salary"])
plt.show()
```

---

## Detect Using IQR

```python
Q1 = df["Salary"].quantile(0.25)
Q3 = df["Salary"].quantile(0.75)

IQR = Q3 - Q1

lower_limit = Q1 - 1.5 * IQR
upper_limit = Q3 + 1.5 * IQR
```

---

## Display Outliers

```python
outliers = df[
    (df["Salary"] < lower_limit) |
    (df["Salary"] > upper_limit)
]
```

---

## Remove Outliers

```python
df = df[
    (df["Salary"] >= lower_limit) &
    (df["Salary"] <= upper_limit)
]
```

---

## Detect Using Z-Score

```python
from scipy.stats import zscore

z_scores = zscore(df["Salary"])
```

---

## Key Points

- Do not remove every outlier.
- Verify whether the value is an error or a valid observation.
- IQR is commonly used in EDA.

---

## Summary

Outlier detection helps identify unusual observations that may affect analysis and model performance.