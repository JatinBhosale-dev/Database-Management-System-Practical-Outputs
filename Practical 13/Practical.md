# Practical 13: Implement PL/SQL Program Using Iterative Statements

**Question:** Implement PL/SQL program using Iterative Statements.

## 1. Concept Overview

Iterative statements (Loops) allow you to execute a block of SQL code multiple times until a specific condition is met. In MySQL Stored Procedures, the most common looping structures are:
*   **WHILE Loop:** Executes as long as a specified condition is true. The condition is checked at the *beginning* of the loop.
*   **REPEAT Loop:** Executes until a specified condition becomes true. The condition is checked at the *end* of the loop (similar to a do-while loop in C/Java).
*   **LOOP:** A basic loop that runs infinitely until it hits a `LEAVE` statement.

*Terminal Reminder:* Just like with conditional statements, you must use the `DELIMITER` command to change the statement terminator so MySQL doesn't execute the procedure prematurely.

---

## 2. Terminal & SQL Execution Steps

**Step 1: Accessing MySQL in Ubuntu Terminal**
Open your terminal (`Ctrl + Alt + T`) and log into the MySQL monitor.

```bash
mysql -u root -p
