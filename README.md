# Library_Management system

## Project Overview
This project implements a Library Management System using MySQL. The system is designed to manage books, members, loans, genres, and authors. It supports key functionalities such as tracking book availability, managing member information, recording borrowing history, and handling relationships between books and authors.

## Features
- **Books**: Tracks books with details like title, author, genre, ISBN, publication year, and availability.
- **Members**: Manages library members, including their personal details and membership type (Basic or Premium).
- **Genres**: Categorizes books into genres (e.g., Fiction, Non-Fiction).
- **Authors**: Stores information about book authors.
- **Book-Author Relationship**: Supports many-to-many relationships between books and authors.
- **Loans**: Records borrowing history, including loan dates and return dates.

## Database Schema
The database schema includes the following tables:
1. **Books**
   - `book_id`: Unique identifier for each book.
   - `title`: Title of the book.
   - `isbn`: International Standard Book Number.
   - `publication_year`: Year of publication.
   - `availability`: Indicates if the book is available for borrowing.
   - `genre_id`: Foreign key linking to the `Genres` table.

2. **Members**
   - `member_id`: Unique identifier for each member.
   - `first_name`: Member's first name.
   - `last_name`: Member's last name.
   - `email`: Member's email (unique).
   - `phone_number`: Member's phone number.
   - `membership_type`: Type of membership (Basic or Premium).

3. **Genres**
   - `genre_id`: Unique identifier for each genre.
   - `name`: Name of the genre.

4. **Authors**
   - `author_id`: Unique identifier for each author.
   - `first_name`: Author's first name.
   - `last_name`: Author's last name.
   - `biography`: Brief biography of the author.

5. **Book_Authors**
   - A junction table to handle the many-to-many relationship between `Books` and `Authors`.

6. **Loans**
   - Tracks borrowing history, linking `Books` and `Members`.
   - Includes `loan_date` and `return_date`.

## How to Run/Setup
### Prerequisites
- Install MySQL Server.
- Install a MySQL client (e.g., MySQL Workbench or command-line client).
- import the Library_management.sql file into your machine and its ready to run.

**ERD**
Below is a visual representation of the database schema:

![alt text](<ERD IMAGE.png>)

Contact
For any questions or feedback, feel free to reach out:

Name : [KLAAS]
Email : [tshupianematlou@gmail.com]

