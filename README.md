CREATE DATABASE college_demo → Creates a database named college_demo.
USE college_demo → Selects the college_demo database for further operations.
CREATE TABLE department → Creates a table to store department information.
dept_id INT PRIMARY KEY → Each department must have a unique ID, and it cannot be empty.
dept_name VARCHAR(50) UNIQUE NOT NULL → Department names can contain up to 50 characters, cannot be empty, and cannot be repeated.
CREATE TABLE student → Creates a table to store student information such as roll number, name, email, and department.
Student constraints → roll_no is unique, name cannot be empty, and email cannot be duplicated.
CREATE TABLE course → Creates a table for storing course details such as course ID, course name, and department.
Foreign Keys → Student and Course dept_id values must match an existing dept_id in the department table.
CREATE TABLE enrollment → Stores which student takes which course, their semester, and grade. Semester must be 1–8, and the combination of roll_no + course_id + semester must be unique.
