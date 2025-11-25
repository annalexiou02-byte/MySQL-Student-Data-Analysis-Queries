# 💾 MySQL Project: Advanced Data Querying and Management

**Institution:** Athens University of Economics and Business (AUEB)
**Project Focus:** Database Management and SQL Query Optimization


## 💡 Project Summary

This project involves the creation and manipulation of a single database table (`student`) using MySQL. It demonstrates foundational database operations (INSERT, UPDATE) and focuses heavily on crafting complex **SELECT queries** to extract meaningful insights and perform statistical analysis on simulated student academic data (Name, Age, GPA, Mentor).

## 🛠️ Database Setup and Data Insertion (DDL/DML)

The `homework2.sql` script begins with the following steps:

1.  **Database Selection:** `use aueb;`
2.  **Initial Query:** `select * from student;`
3.  **Data Population (10 Records):** Insertion of 10 student records, including names (e.g., ANNA ALE, MANOS SIF) and academic metrics (AGE, GPA, MENTOR).
4.  **Data Modification:** A single `UPDATE` query modifies all male students' mentor ID to '1'.

## 🔎 Key Analytical Queries Demonstrated

The project includes several key queries demonstrating various SQL functionalities for data analysis:

| Query # | SQL Functionality | Objective |
| :--- | :--- | :--- |
| **#1** | `MAX()`, Subquery | Retrieve the `ID` and `NAME` of the student with the **highest GPA**. |
| **#2** | `ORDER BY`, `LIMIT` | Retrieve the `ID` and `NAME` of the **top 3 students** ordered by GPA. |
| **#3** | `AVG()`, Subquery | Retrieve the `ID`, `NAME`, and `GPA` of all students whose GPA is **higher than the class average**. |
| **#4** | `MAX()` - `MIN()`, `WHERE` | Calculate the **age difference** between the oldest and youngest male students. |
| **#5** | `MIN()`, Nested Subquery | Retrieve the `ID`, `NAME`, and `GPA` of the female student with the **lowest GPA**. |
| **#6** | `AVG()`, `WHERE` (Range) | Calculate the **average GPA** for students aged **21 to 24** (age > 20 AND age < 25). |

## 🤝 Mentor/Group Analysis Queries

The script includes advanced queries focused on analyzing mentor performance and group metrics:

| Query # | SQL Functionality | Objective |
| :--- | :--- | :--- |
| **#8** | `JOIN` (Implicit), `AVG()`, `GROUP BY` | Calculate the **average GPA** achieved by the mentees assigned to each mentor (`id_mentor`). |
| **#9** | `HAVING`, `AVG()` | Identify the mentor `ID`s whose assigned mentees have an **average GPA below 3.5**. |
| **#10** | `HAVING`, Nested `AVG()` Subquery | Identify the mentor `ID`s whose assigned mentees have an average GPA **below the overall student GPA average**. |

---

