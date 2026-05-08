# Practical 3: Create Tables with Primary Key, Foreign Key, and Other Constraints

**Question:** Create tables with primary key and foreign key and other constraints.

## 1. Constraints Overview

In SQL, constraints are rules applied to table columns to enforce data accuracy and reliability. For this practical, we will demonstrate the following constraints in a single schema:
*   **PRIMARY KEY:** Uniquely identifies each row in a table.
*   **FOREIGN KEY:** Establishes a link/relationship between two tables.
*   **NOT NULL:** Ensures a column cannot accept a NULL value.
*   **UNIQUE:** Ensures all values in a column are entirely distinct from one another.
*   **CHECK:** Ensures all values in a column satisfy a specific logical condition (e.g., Age must be 18 or older).
*   **DEFAULT:** Sets a fallback value for a column if no data is provided during insertion.

---

## 2. Terminal & SQL Execution Steps

**Step 1: Accessing MySQL in Ubuntu Terminal**
Open your terminal (`Ctrl + Alt + T`) and log into the MySQL monitor.

```bash
mysql -u root -p
