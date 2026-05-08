# Practical 15: Create Implicit and Explicit Cursors

**Question:** Create Implicit and Explicit Cursors.

## 1. Concept Overview

A **Cursor** is a temporary work area created in the system memory when a SQL statement is executed. It holds the data retrieved from the database and allows you to manipulate it row by row.

*   **Implicit Cursors:** MySQL automatically creates these for single-row `DML` operations (`INSERT`, `UPDATE`, `DELETE`). You don't declare them. You can check how many rows an implicit cursor affected by using the `ROW_COUNT()` function.
*   **Explicit Cursors:** You must explicitly define these inside a Stored Procedure when you need to process a query that returns *multiple rows*, one row at a time. The standard lifecycle of an explicit cursor is: `DECLARE` -> `OPEN` -> `FETCH` (in a loop) -> `CLOSE`.

---

## 2. Terminal & SQL Execution Steps

**Step 1: Accessing MySQL in Ubuntu Terminal**
Open your terminal (`Ctrl + Alt + T`) and log into the MySQL monitor.

```bash
mysql -u root -p
