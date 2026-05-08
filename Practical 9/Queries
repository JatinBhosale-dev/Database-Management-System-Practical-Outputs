-- Setup: Create database, tables, and insert sample data designed for testing joins
CREATE DATABASE IF NOT EXISTS Practical9DB; USE Practical9DB;
CREATE TABLE Department (DeptID INT PRIMARY KEY, DeptName VARCHAR(50));
CREATE TABLE Student (RollNo INT PRIMARY KEY, Name VARCHAR(50), DeptID INT);

-- Insert data (Notice Dept 103 and 104 have no students, and Vikram has no department)
INSERT INTO Department VALUES (101, 'Computer'), (102, 'IT'), (103, 'Mechanical'), (104, 'Civil');
INSERT INTO Student VALUES (1, 'Aditya', 101), (2, 'Rahul', 102), (3, 'Sneha', 101), (4, 'Vikram', NULL);

-- 1. INNER JOIN: Find students who have an assigned department (Excludes Vikram, Mechanical, and Civil)
SELECT Student.RollNo, Student.Name, Department.DeptName FROM Student INNER JOIN Department ON Student.DeptID = Department.DeptID;

-- 2. LEFT JOIN: Show ALL students, and their departments if they have one (Vikram will show NULL for DeptName)
SELECT Student.RollNo, Student.Name, Department.DeptName FROM Student LEFT JOIN Department ON Student.DeptID = Department.DeptID;

-- 3. RIGHT JOIN: Show ALL departments, and the students in them (Mechanical and Civil will show NULL for Student details)
SELECT Student.RollNo, Student.Name, Department.DeptName FROM Student RIGHT JOIN Department ON Student.DeptID = Department.DeptID;

-- 4. FULL OUTER JOIN (MySQL Equivalent): Show everything! All students and all departments, matching where possible.
SELECT Student.RollNo, Student.Name, Department.DeptName FROM Student LEFT JOIN Department ON Student.DeptID = Department.DeptID UNION SELECT Student.RollNo, Student.Name, Department.DeptName FROM Student RIGHT JOIN Department ON Student.DeptID = Department.DeptID;
