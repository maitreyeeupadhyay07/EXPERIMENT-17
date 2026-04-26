

---

# 📊 Experiment 17: Basic Charts and Visual Encoding in Python

---

## 🎯 Aim

To study and implement different basic charts and visual encoding techniques using Python libraries such as Matplotlib, Seaborn, Pandas, and NumPy for effective graphical representation of data.

---

## 📚 Theory

Data visualization refers to the graphical representation of data through charts, graphs, and plots. It converts raw numerical information into meaningful visuals, making it easier to understand trends, comparisons, relationships, and distributions.

Python offers several powerful libraries for visualization:

* **Matplotlib** → A fundamental plotting library used for creating static charts
* **Seaborn** → An advanced statistical visualization library built on Matplotlib
* **Pandas** → Used for creating and managing structured datasets
* **NumPy** → Used for numerical computations such as calculating averages and means

This experiment demonstrates various chart types and visual encoding methods using these libraries.

---

## 🔹 1. Dataset Creation using Pandas

A structured dataset was created using Python dictionaries and converted into a DataFrame using `pd.DataFrame()`.

The dataset included the following fields:

* Days
* Study_Hours
* Marks
* Attendance
* Sleep_Hours
* Assignments_Completed

This student dataset was used for creating line charts, bar charts, histograms, and scatter plots.

Additionally, another dataset related to business data was created, which included:

* Days
* Region
* Sales
* Profit
* Customers
* Category

This dataset was used for Seaborn-based visualizations.

---

## 🔹 2. Line Chart

A line chart is used to represent trends or variations over time or categories.

The function `plt.plot(x, y)` was used to connect data points with straight lines. Markers such as `marker='*'` were used to highlight individual points.

This chart plotted Study Hours against Days to observe how study time changed throughout the week.

Additional functions used:

* `plt.title()` → Adds a title
* `plt.xlabel()` → Labels the x-axis
* `plt.ylabel()` → Labels the y-axis
* `plt.show()` → Displays the chart

---

## 🔹 3. Multi-Line Chart

Multiple lines can be displayed on a single graph by calling `plt.plot()` multiple times.

Study Hours and Marks were plotted together using different colors and markers. The function `plt.legend()` was used to distinguish between the lines.

This chart allows comparison of two variables simultaneously.

The function `plt.figure(figsize=(7,4))` was used to set the size of the chart.

---

## 🔹 4. Bar Chart

A bar chart is used to compare values across different categories using rectangular bars.

The function `plt.bar(x, y)` was used to plot Marks against Days.

Bar charts are effective for comparing discrete categories such as marks across weekdays.

The parameter `color='green'` was used to style the bars.

---

## 🔹 5. Bar Chart with Value Labels

An enhanced bar chart was created by displaying numerical values above each bar.

This was achieved using:

* `bar.get_height()` → Retrieves the height of each bar
* `plt.text()` → Displays the value above the bar

The function `plt.grid(axis='y')` was used to add horizontal grid lines for improved readability.

This chart provides both visual and precise numerical comparison.

---

## 🔹 6. Histogram

A histogram is used to represent the frequency distribution of continuous numerical data.

The function `plt.hist(data, bins=5)` was used to group marks into intervals.

Parameters used:

* `bins=5` → Number of intervals
* `edgecolor='black'` → Adds borders to bars
* `alpha=0.7` → Controls transparency

This chart helps in understanding the spread and concentration of data.

---

## 🔹 7. Histogram with Mean Line

An improved histogram was created by adding a vertical line representing the mean.

The mean was calculated using:

`np.mean(data)`

The function:

`plt.axvline(mean_value)`

was used to draw a vertical dashed red line indicating the average value.

Additional styling:

* `linestyle='--'`
* `linewidth=2`

This visualization helps compare the distribution of data with its average.

---

## 🔹 8. Scatter Plot

A scatter plot is used to show the relationship between two numerical variables.

The function `plt.scatter(x, y)` was used to plot Study Hours against Marks.

Each point represents an individual observation.

An upward trend from left to right indicates a positive correlation.

This type of graph is useful for analyzing relationships between variables.

---

## 🔹 9. Conditional Scatter Plot (Visual Encoding)

Visual encoding involves using visual elements such as color, shape, or size to represent additional information.

A scatter plot was created where points were colored based on results:

* Red → Fail
* Green → Pass

This was achieved using the `c=` parameter in `plt.scatter()`.

Thus, three variables were represented:

* X-axis → Study Hours
* Y-axis → Marks
* Color → Result

---

## 🔹 10. Seaborn Line Plot

The function `sns.lineplot(x=, y=, data=)` was used to create a line chart for Sales versus Days.

Seaborn automatically produces cleaner and more visually appealing charts compared to basic Matplotlib.

This chart was used to analyze sales trends.

---

## 🔹 11. Seaborn Histogram

The function `sns.histplot(data, kde=True)` was used to display the distribution of Sales.

The parameter `kde=True` adds a smooth density curve over the histogram.

This helps in understanding the shape and pattern of the distribution.

---

## 🔹 12. Seaborn Scatter Plot

The function `sns.scatterplot(x=, y=, data=)` was used to plot Sales against Profit.

This chart helps determine whether higher sales correspond to higher profit.

Seaborn plots are more visually appealing and easier to interpret.

---

## 📊 Output Summary

The following visualizations were successfully generated:

* Line Chart
* Multi-Line Comparison Chart
* Bar Chart
* Labelled Bar Chart
* Histogram
* Histogram with Mean Line
* Scatter Plot
* Conditional Scatter Plot
* Seaborn Line Plot
* Seaborn Histogram
* Seaborn Scatter Plot

---

## 📈 Comparison: Matplotlib vs Seaborn

| Feature            | Matplotlib | Seaborn    |
| ------------------ | ---------- | ---------- |
| Customization      | High       | Medium     |
| Simplicity         | Medium     | High       |
| Appearance         | Basic      | Attractive |
| Statistical Charts | Limited    | Excellent  |

---

## ✅ Conclusion

This experiment successfully demonstrated various basic chart types and visual encoding techniques using Python. Matplotlib provided high flexibility and customization, while Seaborn offered more refined and visually appealing statistical plots. These tools are essential for data analysis, enabling effective representation of trends, comparisons, distributions, and relationships.

---
