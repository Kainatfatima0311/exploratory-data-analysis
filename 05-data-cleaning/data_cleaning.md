# Data Cleaning

## Definition

Data Cleaning is the process of correcting, formatting, and standardizing data before analysis.

---

## Why is Data Cleaning Important?

- Improves data quality
- Removes inconsistencies
- Prevents incorrect analysis
- Improves machine learning performance

---

## Remove Extra Spaces

```python
df["Name"] = df["Name"].str.strip()
```

---

## Convert to Lowercase

```python
df["City"] = df["City"].str.lower()
```

---

## Convert to Title Case

```python
df["City"] = df["City"].str.title()
```

---

## Replace Incorrect Values

```python
df["City"] = df["City"].replace("Lhore","Lahore")
```

---

## Display Unique Values

```python
df["City"].unique()
```

---

## Count Unique Values

```python
df["City"].nunique()
```

---

## Frequency Count

```python
df["Department"].value_counts()
```

---

## Convert Data Type

```python
df["Age"] = df["Age"].astype(int)
```

---

## Convert Date

```python
df["Joining_Date"] = pd.to_datetime(df["Joining_Date"])
```

---

## Key Points

- Clean data before visualization.
- Standardize categorical values.
- Remove unnecessary spaces.
- Ensure correct data types.

---

## Summary

Data Cleaning prepares raw data for accurate analysis and machine learning.