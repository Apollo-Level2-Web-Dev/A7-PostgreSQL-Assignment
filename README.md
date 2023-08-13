# PostgreSQL Assignment

### Assignment Description

In this assignment, you will work with PostgreSQL, a powerful open-source relational database management system. Your task involves creating 03 tables based on the provided sample data and then writing and executing queries to perform various database operations such as creating, reading, updating, and deleting data. Additionally, you will explore concepts like LIMIT and OFFSET, JOIN operations, GROUP BY, aggregation and LIKE.

## Instructions:

### Database Setup:

- Install PostgreSQL on your system if not already installed.
- Create a fresh database titled **"university_db"** or any other appropriate name.

## Table Creation:

Create a **"students"** table with the following fields:

- `student_id` (Primary Key): Integer, unique identifier for students.
- `student_name`: String, representing the student's name.
- `age`: Integer, indicating the student's age.
- `email`: String, storing the student's email address.

Create a **"courses"** table with the following fields:

- `course_id` (Primary Key): Integer, unique identifier for courses.
- `course_name`: String, indicating the course's name.
- `credits`: Integer, signifying the number of credits for the course.

Create an **"enrollment"** table with the following fields:

- `enrollment_id` (Primary Key): Integer, unique identifier for enrollments.
- `student_id` (Foreign Key): Integer, referencing student_id in "Students" table.
- `course_id` (Foreign Key): Integer, referencing course_id in "Courses" table.

## Sample Data

- Insert the following sample data into the **"students"** table:

| student_id | student_name | age | email             |
|------------|--------------|-----|-------------------|
| 1          | Alice        | 22  | alice@example.com|
| 2          | Bob          | 21  | bob@example.com  |
| 3          | Charlie      | 23  | charlie@example.com|
| 4          | David        | 20  | david@example.com|
| 5          | Eve          | 24  | newemail@example.com|
| 6          | Rahim        | 23  | rahim@gmail.com  |

- Insert the following sample data into the **"courses"** table:

| course_id | course_name    | credits |
|-----------|----------------|---------|
| 1         | Programming    | 3       |
| 2         | Algorithms     | 4       |
| 3         | Databases      | 3       |


- Insert the following sample data into the **"enrollment"** table:

| enrollment_id | student_id | course_id |
|---------------|------------|-----------|
| 1             | 1          | 1         |
| 2             | 1          | 2         |
| 3             | 2          | 1         |
| 4             | 3          | 2         |



## Execute SQL queries to fulfill the ensuing tasks:

### Query 1:
Insert a new student record with the following details:

- Name: YourName
- Age: YourAge
- Email: YourEmail


### Query 2:
Retrieve the names of all students who are enrolled in the course titled 'Programming'.

**Sample Output:**
| student_name |
|--------------|
| Alice        |
| Bob        |

### Query 3:
Update the email address of the student with the highest age to 'newemail@ph.com'.

### Query 4:
Delete all courses that have no students enrolled.

### Query 5:
Retrieve the names of students in batches of 2, starting from the 3rd student.

**Sample Output:**
| student_name |
|--------------|
| Charlie      |
| David        |

### Query 6:
Retrieve the course names and the number of students enrolled in each course.

**Sample Output:**
| course_name    | students_enrolled |
|----------------|-------------------|
| Programming    | 2                 |
| Algorithms     | 2                 |


### Query 7:
Calculate and display the average age of all students.

**Sample Output:**
| average_age |
|-------------|
| 22.2857142857142857       |

### Query 8:
Retrieve the names of students whose email addresses contain 'example.com'.

**Sample Output:**
| student_name |
|--------------|
| Alice        |
| Bob          |
| Charlie      |
| David        |


**Prepare the SQL code for table creation, sample data insertion, and the seven queries in a text document or your preferred format. Include comments explaining each query's purpose and functionality. Save your document as "PostgreSQL_Assignment.sql" or any other appropriate name.**

## Questions:
1. What is PostgreSQL?
2. What is the purpose of a database schema in PostgreSQL?
3. Explain the primary key and foreign key concepts in PostgreSQL.
4. What is the difference between the VARCHAR and CHAR data types?
5. Explain the purpose of the WHERE clause in a SELECT statement.
6. What are the LIMIT and OFFSET clauses used for?
7. How can you perform data modification using UPDATE statements?
8. What is the significance of the JOIN operation, and how does it work in PostgreSQL?
9. Explain the GROUP BY clause and its role in aggregation operations.
10. How can you calculate aggregate functions like COUNT, SUM, and AVG in PostgreSQL?
11. What is the purpose of an index in PostgreSQL, and how does it optimize query performance?
12. Explain the concept of a PostgreSQL view and how it differs from a table.

**Provide detailed answers to these questions in your assignment GitHub repository's README file as part of your assignment submission.**