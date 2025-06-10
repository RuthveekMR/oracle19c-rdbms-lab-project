# 📚 RDBMS Lab Project — Oracle 19c  
*Complete End-to-End SQL & PL/SQL Project based on IV BTech Lab Manual*

![Oracle](https://img.shields.io/badge/Database-Oracle%2019c-blue)  
![SQL](https://img.shields.io/badge/Language-SQL%20%26%20PL%2FSQL-orange)  
![Project](https://img.shields.io/badge/Type-End--to--End--Lab--Project-success)

---

## 📌 Project Description

This project implements a complete **Relational Database Management System (RDBMS)** using Oracle Database 19c Enterprise Edition Release 19.0.0.0.0 - Production (Version 19.3.0.0.0), based on the **IV BTech Database Lab Manual**.  
It covers the entire lifecycle of building a database application — from schema design, data manipulation, complex querying, procedural programming (PL/SQL), to cursors, views, procedures, functions, triggers, exception handling, and more.

**Note:** The separate *Mini Project (Week 10-11)* component was not included. This project documents **Weeks 1–9** in a fully functional, end-to-end manner.

---

## 🏢 Business Domain

This database models a **Software Development / IT Consulting Company** that manages:

- Employees with various designations and qualifications
- Employee skills and skill experience
- Clients (International and Domestic)
- Projects led by employees and worked on by employees
- Work experience of employees on projects and ratings given by clients
- Family dependents of employees
- Medical policies associated with employees
- Salary components of employees (including incentives and payroll details)
- Account operations (used for learning PL/SQL transaction processing)

Through this schema, the project demonstrates how a relational database can be used to model a complete corporate scenario with **complex relationships and business rules**, fully implemented using **SQL and PL/SQL** in Oracle 19c.

---

## 📖 Table of Contents

- [Project Description](#-project-description)
- [Business Domain](#-business-domain)
- [Technologies Used](#-technologies-used)
- [Schema Design](#-schema-design)
- [Features Implemented](#-features-implemented)
- [Challenges & Learnings](#-challenges--learnings)
- [How to Run](#-how-to-run)
- [Author](#-author)
- [References](#-references)

---

## 💻 Technologies Used

- **Database:** Oracle Database 19c Enterprise Edition Release 19.0.0.0.0 - Production (Version 19.3.0.0.0)  
- **Language:** SQL, PL/SQL  
- **Tools:** Oracle SQL*Plus / Oracle SQL Developer / Terminal  
- **Reference Materials:** LMS Notes, Lectures, W3Schools, Oracle Docs, ChatGPT (for validating code logic)

---

## 🗂 Schema Design

The following tables were created with appropriate constraints (Primary Key, Foreign Key, Unique, Check, etc.):

- `EMP`  
- `PRJ_DETAILS`  
- `SKILL`  
- `CLIENT`  
- `FAMILY_DEPENDENTS`  
- `MEDICAL_POLICY`  
- `PAY_CHECK`  
- `EMP_SKILL`  
- `WORK_EXP`  
- `ACCOUNT` (Created for PL/SQL based procedures)

---

## 🚀 Features Implemented

### 1️⃣ Schema Creation (DDL)
- Tables created with Primary Keys, Foreign Keys, Check Constraints, Unique Constraints.
- Complex constraints added using `ALTER TABLE`.

### 2️⃣ Data Manipulation (DML)
- Bulk `INSERT ALL` operations.
- `UPDATE`, `DELETE`, `ROLLBACK`, and `COMMIT` operations with constraint validation.

### 3️⃣ Advanced SQL Queries
- Joins: Inner, Natural  
- Subqueries: Scalar, Correlated  
- Set Operators: `UNION`, `INTERSECT`, `MINUS`  
- Aggregation: `GROUP BY`, `HAVING`, `COUNT`, `SUM`  
- Functions: `TO_CHAR`, `MONTHS_BETWEEN`, `ADD_MONTHS`, `LPAD`, `RPAD`, `REPLACE`, `NEXT_DAY`, etc.

### 4️⃣ Views
- Created Views like `emp_skill_experience`, `emp_designation`.

### 5️⃣ PL/SQL Programming
- **Anonymous Blocks** for:
  - Reverse a number
  - Palindrome check
  - Display Employee Details
  - Count vowels/consonants/numbers/special characters
  - Salary Processing with `Pay_Check`
  - Exception Handling on `ACCOUNT` table operations
  - Project leader and Project Name display for budget-efficient projects
  - Dynamic Email Generation using cursors
  - Parameterized Cursor for Client Rating and Work Exp queries
- **Procedures**:
  - `account_balance` → Withdraw with minimum balance validation
  - `project_marvel` → Display employees with skill experience >= 12 for a skill
  - `additional_budget` → Calculate additional budget needed based on project end date difference
- **Functions**:
  - `compute_incentive` → Calculate incentive for employee based on project rating
  - `country_code` → Return employee names working for clients in a country (based on phone code)
  - `generate_email` → Dynamically generate corporate email based on name and ID
- **Triggers**:
  - `salary_increment` → Allow salary increment only for valid designations and ranges
  - `project_modify` → Enforce company policy on project lead eligibility (skill experience ≥ 18)

### 6️⃣ Cursors
- Explicit cursors with `LOOP` and `FOR LOOP`.
- Parameterized cursors for dynamic queries.

### 7️⃣ Exception Handling
- Custom exception handling in:
  - `account_balance` procedure
  - `project_marvel` procedure
  - `additional_budget` procedure
  - Triggers and Functions

---

## 🌟 Challenges & Learnings

> In this project, I found that the *starting step of each week* was often time-consuming and challenging. However, once I got started, I was able to progress smoothly through each week's tasks. To prepare effectively, I made sure to study the relevant concepts beforehand — using LMS notes, lecture notes, teacher explanations, **W3Schools**, and **ChatGPT** (mainly to verify if there was a better way to write certain queries and to confirm the correctness of my logic).  
> Through this approach, I developed a *deep understanding* of SQL and PL/SQL concepts — not just remembering syntax, but grasping the "why" behind each concept and knowing when and how to apply them. Now, these skills feel second nature to me; even after a break of a few months, I am confident that a quick review would bring all concepts back into my mind due to this solid foundation.

---

## ⚙️ How to Run

1. Clone the repository or download the SQL files.
2. Connect to Oracle 19c database using SQL*Plus or SQL Developer.
3. Run the **Table Creation** scripts.
4. Run the **INSERT** scripts to populate the database.
5. Run **DML Queries** to test data manipulations.
6. Run **Advanced Queries**, **Views**, **Procedures**, **Functions**, **Triggers**, and **PL/SQL blocks** to explore the full project functionality.

---

## 👤 Author

**Ruthveek M R**  
- BTech Data Science & Engineering, MIT Manipal  
- Email: ruthmys123@gmail.com  
- GitHub: [Your GitHub Profile Link] *(You can update this link once you upload the project)*

---

## 🌐 References

- IV BTech Lab Manual (Database Lab DSE 2241)  
- Ivan Bayross, *SQL, PL/SQL — The Programming Language of Oracle*  
- W3Schools  
- Oracle Docs  
- LMS Materials & Faculty Sessions  
- ChatGPT (used to compare alternative query approaches and validate logic)

---

### 🚀 This project is a complete **End-to-End Database Learning Project** (excluding Weeks 10-11 Mini Project) and serves as a strong foundation for professional SQL & PL/SQL development.

---

## 📁 Folder Structure

Root/
├── README.md
├── IV_BTech_labmanual_DBS_2025.docx.pdf
├── week1_soln (create_tables).txt
├── week2_soln (alter_tables).txt
├── week3_soln (insert_update_delete).txt
├── week4_soln (basic_queries).txt
├── week5_solution (advanced_queries_and_views).txt
├── week6_soln (Built-in Functions).txt
├── week7_soln (PLSQL Cursors and Exception Handling).txt
├── week8_soln (PLSQL Stored Procedures and Functions).txt
├── week9_soln (PLSQL Triggers).txt


