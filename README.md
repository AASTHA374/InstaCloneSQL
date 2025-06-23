# InstaCloneSQL
A backend database design simulating Instagram's core functionality using SQL. Includes schema design, queries, and data integrity handling.

## Features
- Normalized relational schema for users, posts, comments, likes, followers
- Complex joins and aggregation queries
- Foreign key and junction tables for referential integrity
- Sample data for testing

## Tech Stack
- MySQL

## How to Use
- Open the `.sql` file in any SQL IDE (MySQL Workbench / DBeaver / phpMyAdmin)
- Execute schema creation and insert sample data
- Run queries for analysis

## Example Queries
```sql
SELECT username, COUNT(*) FROM posts GROUP BY username;
SELECT users.name, comments.comment FROM comments JOIN users ON comments.user_id = users.id;
