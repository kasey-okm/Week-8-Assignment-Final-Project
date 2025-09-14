# Library Management System Database

## Overview
This project provides a MySQL relational database schema for a Library Management System. It is designed to manage books, authors, genres, members, book copies, and loans, supporting typical library operations.

## Database Structure

- **authors**: Stores author details.
- **genres**: Stores book genres.
- **books**: Stores book information, linked to authors and genres.
- **book_copies**: Tracks individual physical copies of each book.
- **members**: Stores library member information.
- **loans**: Tracks which member has borrowed which book copy and when.

## Relationships

- Each book is written by one author and belongs to one genre.
- Each book can have multiple physical copies.
- Each member can borrow multiple book copies.
- The `loans` table links members to specific book copies.

## Constraints

- Primary keys for all tables.
- Foreign keys to enforce relationships.
- Unique constraints on ISBN and member email.
- Not Null constraints for required fields.

## Usage

1. Run the SQL file (`library_management.sql`) in your MySQL environment.
2. The database and tables will be created with all constraints and relationships.

## Example

To create the schema, use:
```sql
SOURCE /path/to/library_management.sql;
```

## Author

Your Name  
Date: September 2025# Week-8-Assignment-Final-Project