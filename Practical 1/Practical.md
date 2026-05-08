Design any database with at least two entities and relationships between them. Draw suitable ER/EER diagram for the system.

# Practical 1: Database Design and ER Diagram (MySQL on Ubuntu)

**Question:** Design any database with at least two entities and relationships between them. Draw suitable ER/EER diagram for the system.

## 1. ER Diagram Specification

**System:** University Management (Student & Department)

*   **Entities:**
        *   `Department` (Parent Entity)
        *   `Student` (Child Entity)
*   **Attributes:**
        *   **Department:** `DeptID` (Primary Key, underlined), `DeptName`, `HOD`
        *   **Student:** `RollNo` (Primary Key, underlined), `Name`, `Marks`, `City`, `DeptID` (Foreign Key)
*   **Relationship:**
        *   `Belongs_To` (Many-to-One / M:1): Many Students (M) belong to One Department (1).

> **Drawing Note for Practical Record:** Draw rectangles for `Student` and `Department`. Connect them with a diamond labeled `Belongs_To`. Attach attributes as ellipses to their respective entities. Underline `DeptID` and `RollNo` to denote primary keys. Mark the connecting lines with 'M' on the Student side and '1' on the Department side.

---

## 2. Terminal & SQL Execution Steps

**Step 1: Accessing MySQL in Ubuntu Terminal**
Open your terminal (`Ctrl + Alt + T`) and log into the MySQL monitor. 

```bash
# Log in as root user (you will be prompted for your MySQL password)
mysql -u root -p
