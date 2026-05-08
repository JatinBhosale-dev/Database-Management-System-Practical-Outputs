# Practical 11: Create and Manage Views for Faster Access on Relations

**Question:** Create and manage Views for faster access on relations.

## 1. Concept Overview

A **View** in SQL is essentially a "virtual table." It does not store data itself; instead, it saves a specific `SELECT` query. Every time you query the view, the database engine recreates the data dynamically from the underlying base tables. 

Views are incredibly useful for two main reasons:
1.  **Simplification:** They hide complex queries (like multi-table joins) behind a simple virtual table name.
2.  **Security:** They allow you to restrict user access to specific rows or columns of a table rather than giving them access to the entire base table.

---

## 2. Terminal & SQL Execution Steps

**Step 1: Accessing MySQL in Ubuntu Terminal**
Open your terminal (`Ctrl + Alt + T`) and log into the MySQL monitor.

```bash
mysql -u root -p
