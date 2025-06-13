#  Library Management System (Relational Database Design)

This project represents a relational database design for a **Library Management System**. It includes an ERD (Entity-Relationship Diagram), SQL schema for table creation, and optional sample data.

---

##  Overview

The system is designed to manage the circulation of books in a library, covering:

- Book and author relationships
- Book instances (copies)
- Member management
- Book issue/return transactions
- Librarian details

---

## 🗃️ Entity Relationship Diagram (ERD)

![Image](https://github.com/user-attachments/assets/2aa25d76-5873-4e41-b802-ed5c70543693)

---

## 🏗️ Tables & Relationships

### ✔️ Core Tables:
- **Book**: Contains book details (Title, ISBN, Genre, etc.)
- **Author**: Stores author names
- **BookAuthor**: Resolves many-to-many between Book and Author
- **BookInstance**: Represents individual physical copies of books
- **Transaction**: Tracks issuing and returning of books
- **Member**: Library members who borrow books
- **Librarian**: Employees who manage transactions

### 🔗 Key Relationships:
- One Book can have many BookInstances
- One Book can be written by multiple Authors (via BookAuthor)
- One Member can borrow many books (via Transactions)
- Transactions link Books, Members, and Librarians

---

## 📦 Files Included

- `schema.sql`: SQL script to create all tables and relationships
- `sample-data.sql`: (optional) SQL to populate sample rows
- `ERD.png`: Diagram of the database structure
- `README.md`: Description of the project

---

## 🧠 Skills Demonstrated

- Relational database design
- Normalization and data integrity
- ERD creation and understanding of foreign key constraints
- Use of SQL Server or similar RDBMS

---

## 🚀 How to Use

1. Open `schema.sql` in your SQL tool (SSMS, Azure Data Studio, etc.)
2. Run the script to create the database
3. Optionally, run `sample-data.sql` to insert dummy records

---



