# Data Visualization

## Definition

Data Visualization is the graphical representation of data to identify patterns, trends, and insights.

---

## Why is Data Visualization Important?

- Simplifies complex data
- Identifies trends
- Detects outliers
- Supports decision-making
- Improves data interpretation

---

## Common Charts

### Line Plot

```python
plt.plot(df["Experience_Years"], df["Salary"])
```

Shows trends over time or ordered values.

---

### Bar Plot

```python
sns.barplot(data=df, x="Department", y="Salary")
```

Compares numerical values across categories.

---

### Count Plot

```python
sns.countplot(data=df, x="Department")
```

Displays category frequencies.

---

### Histogram

```python
plt.hist(df["Age"], bins=10)
```

Shows numerical distribution.

---

### Box Plot

```python
sns.boxplot(x=df["Salary"])
```

Detects outliers and spread.

---

### Violin Plot

```python
sns.violinplot(data=df, x="Department", y="Salary")
```

Displays distribution and density.

---

### Scatter Plot

```python
sns.scatterplot(data=df, x="Experience_Years", y="Salary")
```

Shows relationships between numerical variables.

---

### Heatmap

```python
sns.heatmap(df.corr(numeric_only=True), annot=True)
```

Visualizes correlations.

---

### Pie Chart

```python
plt.pie(...)
```

Shows percentage distribution.

---

## Best Practices

- Use meaningful titles.
- Label axes clearly.
- Choose the correct chart.
- Avoid unnecessary colors.
- Use readable figure sizes.

---

## Summary

Visualization transforms raw data into understandable insights using charts and graphs.