# Practical 6: Use Set Operators to Perform Different Operations

**Question:** Use Set operators to perform different operations.

## 1. Concept Overview

Set operators are used to combine the results of two or more `SELECT` statements into a single result set. For set operations to work, the queries being combined must have the same number of columns, and the corresponding columns must have compatible data types.

The primary set operators are:
*   **UNION:** Combines the results of two queries and removes duplicate rows.
*   **UNION ALL:** Combines the results of two queries but keeps all duplicate rows.
*   **INTERSECT:** Returns only the rows that are common to both queries.
*   **EXCEPT (or MINUS):** Returns rows from the first query that are not present in the second query.

*Viva Note:* Older versions of MySQL (before version 8.0.31) do not natively support `INTERSECT` and `EXCEPT`. If your Ubuntu system runs an older version, you might need to use `INNER JOIN` (for Intersect) or `LEFT JOIN ... IS NULL` (for Except) as workarounds. The queries below use the standard set operators.

---

## 2. Terminal & SQL Execution Steps

**Step 1: Accessing MySQL in Ubuntu Terminal**
Open your terminal (`Ctrl + Alt + T`) and log into the MySQL monitor.

```bash
mysql -u root -p
