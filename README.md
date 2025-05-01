# Sales
# 📊 Task 7: Basic Sales Summary from SQLite using Python

This project is part of **Data Analyst Internship**. The objective is to use **SQL inside Python** to extract and summarize basic sales information and visualize the results using a bar chart.

---

## ✅ Objective

- Create and connect to a SQLite database (`sales_data.db`)
- Create a table called `sales` and populate it with sample data
- Use **SQL queries** to calculate:
  - Total quantity sold per product
  - Total revenue per product
- Display results using:
  - `print()` statements
  - A **bar chart** using `matplotlib`

---

## 🛠 Tools Used

- **Python**
- **SQLite** (via `sqlite3` module)
- **Pandas**
- **Matplotlib**

---

## 📂 Files Included

- `sales_summary.ipynb` – Main Python notebook containing all code
- `sales_data.db` – SQLite database with one `sales` table (optional)
- `sales_chart.png` – Revenue bar chart saved from the notebook
- `README.md` – This file

---

## 📌 Key SQL Query Used

```sql
SELECT 
    product, 
    SUM(quantity) AS total_qty, 
    SUM(quantity * price) AS revenue 
FROM sales 
GROUP BY product;
---
## Credits
 Parag
