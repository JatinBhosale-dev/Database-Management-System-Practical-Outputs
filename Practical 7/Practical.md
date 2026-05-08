# Practical 7: Implement Queries Using Aggregate Functions

**Question:** Implement queries using Aggregate functions.

## 1. Concept Overview

Aggregate functions perform a calculation on a set of values and return a single value. They are incredibly useful for summarizing data. The most common SQL aggregate functions are:
*   **COUNT():** Returns the number of rows that match a specified criterion.
*   **SUM():** Returns the total sum of a numeric column.
*   **AVG():** Returns the average value of a numeric column.
*   **MIN():** Returns the smallest value in a selected column.
*   **MAX():** Returns the largest value in a selected column.

*Note:* Aggregate functions are often used in conjunction with the `GROUP BY` clause to group the result set by one or more columns.

---

## 2. Terminal & SQL Execution Steps

**Step 1: Accessing MySQL in Ubuntu Terminal**
Open your terminal (`Ctrl + Alt + T`) and log into the MySQL monitor.

```bash
mysql -u root -p
