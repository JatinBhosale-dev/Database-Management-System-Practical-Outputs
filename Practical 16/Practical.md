# Practical 16: Create Stored Procedures for Modularity

**Question:** Create stored procedures for modularity.

## 1. Concept Overview

**Modularity** in programming means breaking down a large, complex system into smaller, manageable, and reusable pieces (modules). In SQL, we achieve this using **Stored Procedures**.

Instead of writing long, complex SQL queries repeatedly in your application, you write the logic once inside a stored procedure and save it in the database. 
Benefits of using stored procedures for modularity include:
*   **Reusability:** Code is written once and called multiple times using the `CALL` command.
*   **Maintainability:** If the business logic changes, you only update the procedure in the database, not everywhere in your application.
*   **Reduced Network Traffic:** Instead of sending hundreds of lines of SQL over the network, you just send a single `CALL ProcedureName()` command.

---

## 2. Terminal & SQL Execution Steps

**Step 1: Accessing MySQL in Ubuntu Terminal**
Open your terminal (`Ctrl + Alt + T`) and log into the MySQL monitor.

```bash
mysql -u root -p
