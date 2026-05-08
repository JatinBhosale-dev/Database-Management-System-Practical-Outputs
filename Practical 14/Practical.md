# Practical 14: Implement PL/SQL Program Based on Exception Handling (Pre-defined Exceptions)

**Question:** Implement PL/SQL program based on Exception Handling (Pre-defined exceptions) application.

## 1. Concept Overview

In MySQL (which uses Stored Procedures as its equivalent to Oracle's PL/SQL), exceptions are called **Conditions**, and we handle them using **Condition Handlers**. 

If a query inside a procedure fails (for example, trying to insert a duplicate Primary Key), it will normally crash the procedure and throw an ugly terminal error. With Exception Handling, we "catch" that predefined error and handle it gracefully, allowing the program to output a friendly message or take corrective action.

We use the syntax: `DECLARE [ACTION] HANDLER FOR [CONDITION]`.
*   **ACTION:** Can be `CONTINUE` (keep running the procedure after the error) or `EXIT` (stop the current code block).
*   **CONDITION:** Can be a generic predefined state like `SQLEXCEPTION`, or a specific error code like `SQLSTATE '23000'` (which specifically means "Duplicate Key Error").

---

## 2. Terminal & SQL Execution Steps

**Step 1: Accessing MySQL in Ubuntu Terminal**
Open your terminal (`Ctrl + Alt + T`) and log into the MySQL monitor.

```bash
mysql -u root -p
