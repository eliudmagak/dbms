ENTITY RELATIONSHIP DIAGRAM (ERD)

ERD
- ERD (Entity Relationship Diagram) is used in a Database Management System (DBMS).
- It represents relational databases and shows how entities relate to one another.

ENTITIES
- Entities represent database tables.
- Examples: Users, Products, Students, Courses.

ATTRIBUTES
- Attributes describe entities.
- Attributes represent the columns of a table.

Example:

Users
├── Customer
├── Seller
└── Admin

Products
Payments (Cart)
Order Details

--------------------------------------------------

RELATIONSHIP

- A relationship describes how two or more entities are associated with one another in a database.
- Relationships help reduce redundancy by connecting related entities.

Example:

Student → Course

--------------------------------------------------

PRIMARY KEY

- A Primary Key is a column in an entity/table used to uniquely identify a record.

Example:

Student
- student_id = 21
- name = Jack
- email = jack@gmail.com

Course
- course_id
- course_name

--------------------------------------------------

FOREIGN KEY

- A Foreign Key is a key imported from another entity to enforce relationships between entities.
- It helps maintain data integrity and reduce redundancy.

Example:

Course
- course_id
- course_name
- student_id

Student
- student_id
- student_name
- age

In this example:
- student_id in Course is a Foreign Key.
- It creates a relationship between Student and Course.

--------------------------------------------------

DEPARTMENT EXAMPLE

Department
- department_id
- department_name

Teacher
- teacher_id
- department_id
- teacher_name
- teacher_experience

Class
- class_id
- teacher_id
- class_name

Student
- student_id
- class_id
- name
- age

--------------------------------------------------

TYPES OF RELATIONSHIPS

1. ONE-TO-ONE (1:1)

- One record in Entity A is associated with one record in Entity B and vice versa.

Example:

Student ↔ Admission

- One student has one admission record.
- One admission record belongs to exactly one student.

Representation:

A ||------|| B

--------------------------------------------------

2. ONE-TO-MANY (1:M)

- One record in Entity A can be associated with many records in Entity B.
- Each record in Entity B belongs to one record in Entity A.

Example:

Class ↔ Student

- One class has many students.
- Each student belongs to one class.

Representation:

A ||------|< B

--------------------------------------------------

3. MANY-TO-ONE (M:1)

- Many records in Entity A are associated with one record in Entity B.

Example:

Student ↔ Course

- Many students can belong to one course.
- One course can have many students.

Representation:

A >|------|| B

--------------------------------------------------

4. MANY-TO-MANY (M:N)

- Many records in Entity A can relate to many records in Entity B.

Example:

Student ↔ Subject

- Many students study many subjects.
- Each subject is studied by many students.

Representation:

A >|------|< B

--------------------------------------------------

SUMMARY

Entity
- Represents a table.

Attribute
- Represents a column in a table.

Primary Key
- Uniquely identifies a record.

Foreign Key
- Connects one table to another.

Relationship
- Defines how entities are associated.

Relationship Types
1. One-to-One (1:1)
2. One-to-Many (1:M)
3. Many-to-One (M:1)
4. Many-to-Many (M:N)
