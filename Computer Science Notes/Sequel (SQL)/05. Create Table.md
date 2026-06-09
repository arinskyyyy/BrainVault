
## Create Table 

`CREATE TABLE` statement creates a brand new table in a database.

```sql
CREATE TABLE companies (
  id INTEGER,
  name TEXT,
  headquarters TEXT,
  year INTEGER
);
```

- used to create an empty table with no data.

**Data Types :**

All the data stored in a database has a type. The data type lets the database know what to expect from each column and determines the kind of interactions that can happen.

Some of the most common data types are:

- `TEXT`: a text string
- `INTEGER`: a positive or negative whole number
- `REAL`: a positive or negative decimal number
- `DATE`: a date format (YYYY-MM-DD)

**Insert Into :**

Use the `INSERT` statement to add a new row into a table: 

```sql
INSERT INTO companies (id, name, headquarters, year)
VALUES (1, 'Twitter', 'San Francisco', 2006);
```

Let’s break this down:

- `INSERT INTO` is a clause that adds the specified row.
- `companies` the name of the table the row is being added to.
- `(id, name, headquarters, year)` is a parameter with the column names that data will be inserted to.
- `VALUES` clause indicates the data being inserted.
- `(1, 'Twitter', 'San Francisco', 2006)` are the values.

After using this statement, there'll be be a new row in `companies` where:

- `id` is 1
- `name` is 'Twitter'
- `headquarters` is 'San Francisco'
- `year` is 2006

We can also add multiple rows like so:

```sql
INSERT INTO companies (id, name, headquarters, year)
VALUES (1, 'Twitter', 'San Francisco', 2006);

INSERT INTO companies (id, name, headquarters, year)
VALUES (2, 'Duolingo', 'Pittsburgh', 2011);

INSERT INTO companies (id, name, headquarters, year)
VALUES (3, 'BeReal', 'Paris', 2020);

INSERT INTO companies (id, name, headquarters, year)
VALUES (4, 'Codedex', 'New York', 2022);
```
