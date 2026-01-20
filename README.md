# sql-joins-internship-task
SQL Intermediate Joins using Chinook Database
# SQL Intermediate – Joins Internship Task

## 📌 Overview
This project demonstrates intermediate SQL skills focusing on **JOIN operations (INNER JOIN, LEFT JOIN)** using the **Chinook SQLite database**.  
The task simulates real-world business queries such as customer order analysis, inactive customer identification, and revenue insights.

---

## 🛠 Tools & Technologies
- **Database**: Chinook (SQLite)
- **Tool**: DB Browser for SQLite
- **Language**: SQL

---

## 📂 Project Files
| File Name | Description |
|----------|-------------|
| `joins_queries.sql` | Contains all SQL JOIN queries with comments |
| `joined_output.csv` | Exported result of joined SQL queries |
| `insights.txt` | Business insights derived from the analysis |


## 🧩 Database Tables Used
- `Customer`
- `Invoice`
- `InvoiceLine`
- `Track`
- `Album`
- `Artist`
- `Genre`

Primary and foreign key relationships were used to ensure accurate joins and data integrity.

---

## 🔍 SQL Concepts Covered
- INNER JOIN
- LEFT JOIN
- Aggregations (`SUM`, `GROUP BY`)
- Aliases for readability
- Date filtering using `WHERE`
- Business-driven query logic


## 📈 Sample Query (INNER JOIN)
```sql
SELECT
    c.FirstName,
    c.LastName,
    i.InvoiceId,
    i.InvoiceDate,
    i.Total
FROM Customer c
INNER JOIN Invoice i
    ON c.CustomerId = i.CustomerId;

