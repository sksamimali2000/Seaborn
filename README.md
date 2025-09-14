# 📊 Seaborn Data Visualization Examples

This project demonstrates various data visualization techniques using the **Seaborn** library in Python, using popular datasets like `tips`, `iris`, and `flights`.

---

## ✅ 1. Categorical Data Visualization (`tips` dataset)

- Visualized relationships between `sex` and `total_bill`.
- Plots used:
  - `catplot` (default scatter)
  - Swarm plot
  - Box plot
  - Boxen plot
  - Violin plot (with `iris` dataset for sepal length & width)

---

## ✅ 2. Time Series Visualization (`flights` dataset)

- Plotted passengers over the years.
- Plots used:
  - `relplot` (line plots with hue & columns)
  - `lineplot`

---

## ✅ 3. Scatter Plot Visualization (`tips` dataset)

- Analyzed relationship between `total_bill` and `tip`.
- Plots used:
  - `relplot` (scatter)
  - `scatterplot`
  - Various combinations of `hue`, `style`, and `col`.

---

## ⚡ Libraries Used
- `seaborn`
- `pandas`
- `matplotlib`

---

## 🚀 Key Insights
- Easy comparison of categorical vs numerical data.
- Time series trends effectively visualized using line plots.
- Scatter plots show relationships and group differences (e.g., smoker vs non-smoker).

---

## 📦 Example Code
```python
import seaborn as sns
import matplotlib.pyplot as plt

sns.set()
df = sns.load_dataset('tips')
sns.catplot(x='sex', y='total_bill', data=df, kind='box', hue='smoker')
plt.show()
