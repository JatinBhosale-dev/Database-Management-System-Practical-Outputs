# Practical 10: Create and Manage Index for Faster Retrieval of Data

**Question:** Create and manage Index for faster a retrival of data.

## 1. Concept Overview

An **Index** in a database is just like the index at the back of a textbook. Instead of scanning every single page (a "full table scan") to find information, the database looks at the index to find the exact location of the data instantly. 

While indexes drastically speed up `SELECT` (search/retrieval) queries, they slightly slow down `INSERT`, `UPDATE`, and `DELETE` operations because the index must also be updated every time the data changes.

There are generally two common types we create manually:
*   **Simple Index:** Just speeds up searching. Duplicates are allowed.
*   **Unique Index:** Speeds up searching AND enforces that every value in that column is unique (e.g., for an Email column).

*Note: Primary Keys automatically get a unique index created for them by default.*

---

## 2. Terminal & SQL Execution Steps

**Step 1: Accessing MySQL in Ubuntu Terminal**
Open your terminal (`Ctrl + Alt + T`) and log into the MySQL monitor.

```bash
mysql -u root -p
