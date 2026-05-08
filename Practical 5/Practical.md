# Practical 5: Implement Pattern Matching and Relational Operators

**Question:** Implement Pattern matching and Relational operators to apply various conditions in query.

## 1. Concept Overview

To filter data accurately in SQL, we use operators within the `WHERE` clause:
*   **Relational Operators:** Used to compare values. Includes `=` (Equal), `>` (Greater than), `<` (Less than), `>=` (Greater than or equal), `<=` (Less than or equal), and `!=` or `<>` (Not equal).
*   **Pattern Matching (LIKE Operator):** Used to search for a specified pattern in a column. It uses two main wildcards:
    *   `%` (Percent sign): Represents zero, one, or multiple characters.
    *   `_` (Underscore): Represents exactly one single character.

---

## 2. Terminal & SQL Execution Steps

**Step 1: Accessing MySQL in Ubuntu Terminal**
Open your terminal (`Ctrl + Alt + T`) and log into the MySQL monitor.

```bash
mysql -u root -p
