# Duplicate Data

## Definition

Duplicate data refers to repeated records in a dataset. These records can affect statistical analysis and machine learning performance.

---

## Why Remove Duplicate Data?

- Improve data quality
- Prevent incorrect analysis
- Avoid biased machine learning models
- Reduce unnecessary storage

---

## Detect Duplicate Rows

```python
df.duplicated()
```

Returns True for duplicate rows.

---

## Count Duplicate Rows

```python
df.duplicated().sum()
```

Counts the total number of duplicate rows.

---

## Display Duplicate Rows

```python
df[df.duplicated()]
```

Displays only duplicate records.

---

## Remove Duplicate Rows

```python
df = df.drop_duplicates()
```

Removes duplicate rows from the dataset.

---

## Remove Duplicates Based on Specific Columns

```python
df.drop_duplicates(subset=["Employee_ID"])
```

Removes duplicates based on a selected column.

---

## Key Points

- Always inspect duplicates before removing them.
- Not every repeated value is a duplicate row.
- Use subset when only specific columns should be checked.

---

## Summary

Duplicate data should be identified and removed carefully to improve dataset quality before analysis.