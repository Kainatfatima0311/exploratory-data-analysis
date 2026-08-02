# Bivariate Analysis

## Definition

Bivariate Analysis is the process of analyzing the relationship between two variables.

---

## Numerical vs Numerical

### Scatter Plot

```python
sns.scatterplot(data=df, x="Experience_Years", y="Salary")
```

Shows the relationship between two numerical variables.

---

## Categorical vs Numerical

### Bar Plot

```python
sns.barplot(data=df, x="Department", y="Salary")
```

Displays average values across categories.

---

### Box Plot

```python
sns.boxplot(data=df, x="Department", y="Salary")
```

Compares distributions across categories.

---

## Correlation

```python
df[["Age","Salary"]].corr()
```

Measures the relationship between numerical variables.

---

## GroupBy

```python
df.groupby("Department")["Salary"].mean()
```

Calculates average salary for each department.

---

## Crosstab

```python
pd.crosstab(df["Gender"], df["Department"])
```

Displays frequency between categorical variables.

---

## Key Points

- Analyze two variables together.
- Use scatter plots for numerical relationships.
- Use bar plots and box plots for categorical comparisons.
- Correlation only applies to numerical data.

---

## Summary

Bivariate Analysis helps understand relationships between two variables and identify useful patterns.