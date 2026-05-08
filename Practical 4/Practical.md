# Practical 4: Execute DML Commands to Manipulate Data using SQL

**Question:** Execute DML Commands to manipulate data using SQL.

## 1. DML (Data Manipulation Language) Overview

DML commands are used to manage and manipulate the actual data (records/rows) stored within your database tables. Unlike DDL, which changes the structure, DML only affects the data itself. The core DML commands are:
*   **INSERT:** To add new rows/records into a table.
*   **UPDATE:** To modify existing data within a table based on a condition.
*   **DELETE:** To remove existing rows from a table based on a condition.
*   **SELECT:** (Technically DQL - Data Query Language, but heavily used alongside DML) To retrieve and view data from the table.

---

## 2. Terminal & SQL Execution Steps

**Step 1: Accessing MySQL in Ubuntu Terminal**
Open your terminal (`Ctrl + Alt + T`) and log into the MySQL monitor.

```bash
mysql -u root -p
