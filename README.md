# ⚽ Football Ticket Booking System - Database Assignment

## 📌 Assignment Overview

This repository contains my submission for the **Football Ticket Booking System** database assignment. The objective of this assignment was to design a relational database, create an Entity Relationship Diagram (ERD), implement SQL queries to solve business scenarios, and demonstrate understanding of fundamental database concepts through viva questions.

---

## 🎯 Learning Objectives

Through this assignment, I practiced and strengthened my understanding of:

* Database design principles
* Entity Relationship Diagram (ERD) modeling
* Primary Keys and Foreign Keys
* Referential and Entity Integrity
* One-to-Many and Many-to-One relationships
* Writing SQL queries using:

  * `JOIN`
  * `LEFT JOIN`
  * `Subqueries`
  * Aggregate functions
  * `HAVING`
  * `COALESCE`
  * `LIKE` and `ILIKE`
  * Pagination using `LIMIT` and `OFFSET`

---

## 🗄️ Database Schema

The system consists of three main tables:

### 1. Users

Stores information about football fans and ticket managers.

**Key Attributes:**

* `user_id` (Primary Key)
* `full_name`
* `email`
* `role`
* `phone_number`

---

### 2. Matches

Stores football match details and ticket availability information.

**Key Attributes:**

* `match_id` (Primary Key)
* `fixture`
* `tournament_category`
* `base_ticket_price`
* `match_status`

---

### 3. Bookings

Records ticket purchase transactions.

**Key Attributes:**

* `booking_id` (Primary Key)
* `user_id` (Foreign Key → Users)
* `match_id` (Foreign Key → Matches)
* `seat_number`
* `payment_status`
* `total_cost`

---

## 🔗 Entity Relationships

The database follows these relationships:

* **One User → Many Bookings**

  * A user can purchase tickets for multiple matches.

* **One Match → Many Bookings**

  * Multiple users can book tickets for the same match.

* **Each Booking → One User and One Match**

  * Every booking belongs to exactly one user and one match.

---

## 📊 ERD (Entity Relationship Diagram)

Public ERD Link:

**https://drive.google.com/file/d/1i1EutV9VntQbw4y5tmERrMCDeRkuyDKr/view?usp=sharing**

The ERD includes:

* Primary Keys (PK)
* Foreign Keys (FK)
* Crow's Foot Cardinality
* Relationship constraints
* Status attributes

---

## 📁 Repository Structure

```text
├── QUERY.sql          # SQL queries for all assignment requirements
├── README.md          # Assignment documentation
└── ERD Link           # Public ERD shared above
```

---

## ✅ Implemented SQL Queries

The `QUERY.sql` file contains solutions for the following tasks:

1. Retrieve available Champions League matches.
2. Search users using pattern matching (`LIKE` / `ILIKE`).
3. Handle NULL payment statuses using `COALESCE`.
4. Display booking information using `INNER JOIN`.
5. Show all users including those without bookings using `LEFT JOIN`.
6. Find bookings with costs above the average using subqueries.
7. Retrieve expensive matches using sorting, `LIMIT`, and `OFFSET`.

---

## 🎤 Viva Preparation

As part of this assignment, I also prepared explanations for database concepts including:

* Foreign Keys and Referential Integrity
* Primary Keys and Entity Integrity
* `WHERE` vs `HAVING`
* Main Query vs Subquery
* LEFT JOIN behavior with unmatched records

---

## 🛠️ Technologies Used

* PostgreSQL
* SQL
* Draw.io / Lucidchart (ERD Design)
* Git & GitHub

---

## 📚 Key Database Concepts Applied

* Primary Key Constraints
* Foreign Key Constraints
* Entity Integrity
* Referential Integrity
* Aggregate Functions
* Subqueries
* Join Operations
* NULL Handling
* Database Relationships

---

## 📝 Reflection

This assignment helped me gain practical experience in designing relational databases and writing SQL queries to solve real-world business problems. It also improved my understanding of how database constraints maintain data consistency and integrity.

Overall, this project strengthened my confidence in database design concepts and SQL query development.

---

## 👨‍💻 Student Submission

**Assignment:** Football Ticket Booking System

**Submitted By:** *Sanjit Sarkar*

**GitHub Repository:** *[\[Add Repository Link Here\]](https://github.com/GitHub-Sanjit/Assignment-RDBMS)*


---

Thank you for reviewing my submission.
