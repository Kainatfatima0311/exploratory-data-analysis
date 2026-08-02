# Multivariate Analysis

## Definition

Multivariate Analysis is the process of analyzing relationships among three or more variables simultaneously.

---

## Correlation Matrix

```python
df.corr(numeric_only=True)
```

Shows relationships between numerical variables.

---

## Heatmap

```python
sns.heatmap(
    df.corr(numeric_only=True),
    annot=True,
    cmap="coolwarm"
)
```

Visualizes correlations.

---

## Pair Plot

```python
sns.pairplot(
    df[
        [
            "Age",
            "Salary",
            "Experience_Years",
            "Performance_Score"
        ]
    ]
)
```

Displays pairwise relationships.

---

## Scatter Plot with Hue

```python
sns.scatterplot(
    data=df,
    x="Experience_Years",
    y="Salary",
    hue="Department"
)
```

Adds a third categorical variable.

---

## GroupBy

```python
df.groupby(
    ["Department","Gender"]
)["Salary"].mean()
```

Calculates grouped averages.

---

## Pivot Table

```python
pd.pivot_table(
    df,
    values="Salary",
    index="Department",
    columns="Gender",
    aggfunc="mean"
)
```

Creates summarized reports.

---

## Key Points

- Analyze multiple variables together.
- Heatmaps simplify correlation analysis.
- Pairplots help identify trends.
- Pivot tables summarize grouped data.

---

## Summary

Multivariate Analysis provides deeper insights by analyzing several variables together.