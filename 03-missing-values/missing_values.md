# Missing Values

## Definition

Missing values are empty or unavailable data entries in a dataset. In Pandas, missing values are usually represented as NaN.

---

## Why Handle Missing Values?

- Improve data quality
- Avoid incorrect analysis
- Increase machine learning performance
- Prevent calculation errors

---

## Detect Missing Values

### Check Missing Values

```python
df.isnull()
```

Returns True for missing values.

---

### Count Missing Values

```python
df.isnull().sum()
```

Counts missing values in each column.

---

### Check Missing Value Percentage

```python
(df.isnull().sum()/len(df))*100
```

Returns missing percentage.

---

## Filling Missing Values

### Mean

```python
df["Age"] = df["Age"].fillna(df["Age"].mean())
```

---

### Median

```python
df["Salary"] = df["Salary"].fillna(df["Salary"].median())
```

---

### Mode

```python
df["City"] = df["City"].fillna(df["City"].mode()[0])
```

---

## Remove Missing Values

```python
df.dropna()
```

Removes rows containing missing values.

---

## Key Points

- Use Mean for normally distributed numerical data.
- Use Median for numerical data with outliers.
- Use Mode for categorical data.
- Drop rows only when appropriate.

---

## Summary

Handling missing values is an essential part of data cleaning in EDA.