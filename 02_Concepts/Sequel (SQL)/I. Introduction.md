
## Structured Query language (SQL or sequel)

**SQL** (short for **S**tructured **Q**uery **L**anguage) is a programming language designed to manage and retrieve data stored in databases.

SQL databases are collections of tables, with rows and columns.

SQL statements, or **queries**, are instructions that the database understands. In other words, queries allow us to retrieve information from a database.

the Asterisk( * ) :

```.sql
SELECT * FROM shows;
```

- `SELECT` retrieves data from a database
- `*` asterisk means all columns.
- `FROM` is a keyword followed by the table name
- `shows` is the name of the table, one is requesting the data from
- the semicolon `;` determines the end of a SQL statement

Specific Columns :

```.sql
SELECT column1, column2, column3
FROM table_name;
```

**Note**: SQL keywords like `SELECT` and `FROM` are not case-sensitive, but it's common to write them in uppercase to distinguish them from column names (`id`, `name`, `genre`) and table names (`shows`), which are written in lowercase.

Unique Values :

```.sql
SELECT DISTINCT genre
FROM shows;
```

- When analyzing the database, to view unique values in a column, instead of duplicates.