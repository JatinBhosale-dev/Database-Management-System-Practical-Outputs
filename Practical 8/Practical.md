# Practical 8: Execute Queries for Ordering and Grouping Data

**Question:** Execute queries for Ordering and Grouping data.

## 1. Concept Overview

Organizing and summarizing data is crucial in database management. We use the following clauses to achieve this:
*   **ORDER BY:** Sorts the result set in either Ascending (`ASC` - default) or Descending (`DESC`) order based on one or more columns.
*   **GROUP BY:** Groups rows that have the same values into summary rows, like "find the number of students in each department". It is almost always used with aggregate functions (`COUNT`, `MAX`, `MIN`, `SUM`, `AVG`).
*   **HAVING:** Acts like a `WHERE` clause, but it is specifically used to filter records *after* they have been grouped by the `GROUP BY` clause.

---

## 2. Terminal & SQL Execution Steps

**Step 1: Accessing MySQL in Ubuntu Terminal**
Open your terminal (`Ctrl + Alt + T`) and log into the MySQL monitor.

```bash
mysql -u root -p
