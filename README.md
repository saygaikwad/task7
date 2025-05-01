# task7
 Basic Sales Summary from a Tiny SQLite Database using Python
# Task 7 - Sales Summary using SQLite and Python

## Objective
Analyze a sales dataset using SQL within Python to generate a summary report that includes:

- Total quantity sold per product
- Total revenue generated per product

## Tools Used
- Python (Jupyter Notebook)
- SQLite (`sqlite3`)
- pandas
- matplotlib

## Dataset
The dataset used is `sales_data_sample.csv`, which contains product-level sales records including quantities and prices.

## What I Did
1. Loaded the CSV file into a pandas DataFrame using Jupyter Notebook.
2. Created an in-memory SQLite database using the `sqlite3` library.
3. Inserted the sales data from the DataFrame into an SQLite table.
4. Executed SQL queries to calculate:
   - Total quantity sold per product (`SUM(QUANTITYORDERED)`)
   - Total revenue per product (`SUM(QUANTITYORDERED * PRICEEACH)`)
5. Displayed the result as a DataFrame.
6. Plotted a bar chart to visualize revenue per product using `matplotlib`.
7. Saved the chart as `sales_chart.png`.

## Sample Output

| product   | total_qty | revenue   |
|-----------|-----------|-----------|
| S10_1678  | 230       | 33089.80  |
| S10_1949  | 200       | 30800.00  |
| ...       | ...       | ...       |

This notebook demonstrates how to integrate SQL queries into Python workflows for basic data analysis and reporting.
