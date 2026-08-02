# Univariate Analysis

## Definition

Univariate Analysis is the process of analyzing a single variable to understand its distribution, central tendency, and variability.

---

## Numerical Analysis

### Mean

```python
df["Age"].mean()
```

### Median

```python
df["Age"].median()
```

### Mode

```python
df["Age"].mode()
```

### Minimum

```python
df["Age"].min()
```

### Maximum

```python
df["Age"].max()
```

### Standard Deviation

```python
df["Age"].std()
```

### Variance

```python
df["Age"].var()
```

---

## Categorical Analysis

### Frequency Count

```python
df["Department"].value_counts()
```

---

## Histogram

```python
plt.hist(df["Age"])
plt.show()
```

Shows the distribution of numerical data.

---

## Box Plot

```python
sns.boxplot(x=df["Salary"])
plt.show()
```

Detects outliers and spread.

---

## Count Plot

```python
sns.countplot(x="Department", data=df)
plt.show()
```

Displays category frequencies.

---

## Key Points

- Analyze one variable at a time.
- Numerical and categorical columns use different techniques.
- Box plots help identify outliers.
- Histograms show distributions.

---

## Summary

Univariate Analysis provides a detailed understanding of individual features before exploring relationships between variables.