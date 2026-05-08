# Practical 17: Create Functions for Given Database

**Question:** Create functions for given database.

## 1. Concept Overview

In MySQL, a **User-Defined Function (UDF)** is a stored program that you can pass parameters into, and it **must** return a single value. 

**How is a Function different from a Stored Procedure?** (Crucial Viva Question!)
*   **Execution:** Procedures are executed using the `CALL` statement. Functions are used directly inside standard SQL queries (like `SELECT`, `WHERE`, or `HAVING`).
*   **Return Value:** A procedure does not *have* to return a value (it usually performs actions like `INSERT` or `UPDATE`). A function *must* return exactly one value using the `RETURN` statement.
*   **Usage:** You cannot use a procedure inside a `SELECT` query, but functions are designed specifically for that.

*Note on `DETERMINISTIC`: In MySQL, when you create a function, it is best practice to declare it as `DETERMINISTIC` (meaning if you give it the same input, it will always give the same output) to prevent errors related to binary logging.*

---

## 2. Terminal & SQL Execution Steps

**Step 1: Accessing MySQL in Ubuntu Terminal**
Open your terminal (`Ctrl + Alt + T`) and log into the MySQL monitor.

```bash
mysql -u root -p
