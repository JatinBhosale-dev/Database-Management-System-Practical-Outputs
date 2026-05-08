# Practical 12: Implement PL/SQL Program Using Conditional Statements

**Question:** Implement PL/SQL program using Conditional Statements.

## 1. Concept Overview

*University Note:* "PL/SQL" is technically Oracle's specific procedural language. In MySQL, the exact equivalent is called **Stored Procedures**. Colleges often use the term PL/SQL generally to mean any procedural SQL programming. 

In a Stored Procedure, you can use programming logic like variables and conditional statements (`IF`, `ELSEIF`, `ELSE`) to control the flow of execution. 

**CRITICAL TERMINAL RULE:** Because a procedure contains multiple SQL statements ending in semicolons (`;`), you must temporarily change the MySQL terminal's delimiter (usually to `//`) so it doesn't accidentally execute the code halfway through writing it.

---

## 2. Terminal & SQL Execution Steps

**Step 1: Accessing MySQL in Ubuntu Terminal**
Open your terminal (`Ctrl + Alt + T`) and log into the MySQL monitor.

```bash
mysql -u root -p
