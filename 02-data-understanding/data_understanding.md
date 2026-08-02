# Data Understanding

## Definition

Data Understanding is the process of exploring the structure of a dataset before cleaning or analyzing it.

---

## Why is Data Understanding Important?

- Know the size of the dataset.
- Identify column names.
- Check data types.
- Detect missing values.
- Understand numerical statistics.

---

## Common Pandas Functions

### Load Dataset

```python
pd.read_csv("datasets/sample_data.csv")
```

Loads a CSV dataset into a DataFrame.

---

### head()

Returns the first 5 rows.

```python
df.head()
```

---

### tail()

Returns the last 5 rows.

```python
df.tail()
```

---

### shape

Returns the number of rows and columns.

```python
df.shape
```

Example Output

```
(1000, 12)
```

Meaning:

- 1000 rows
- 12 columns

---

### columns

Displays all column names.

```python
df.columns
```

---

### dtypes

Shows the data type of every column.

```python
df.dtypes
```

---

### info()

Provides complete dataset information.

```python
df.info()
```

Includes:

- Number of rows
- Number of columns
- Data types
- Missing values
- Memory usage

---

### describe()

Displays statistical summary of numerical columns.

```python
df.describe()
```

Includes:

- Count
- Mean
- Standard Deviation
- Minimum
- Maximum
- Quartiles

---

## Key Points

- Always understand the dataset before cleaning.
- Check data types carefully.
- Use info() to identify missing values.
- Use describe() to understand numerical features.

---

## Summary

Data Understanding is the first coding step in every EDA project. It helps understand the dataset structure before further analysis.