
**Introduction**

A **join** lets us combine rows from two or more tables, based on a related column.

There are several types of joins in SQL, each serving a different purpose:

- `JOIN`
- `LEFT JOIN`
- `RIGHT JOIN`
- `FULL JOIN`
- `UNION`

<p align="center">
  <img src="https://i.imgur.com/0cmu2DP.png" width="400">
</p>

`INNER JOIN OR JOIN`:

<p align="center">
  <img src="https://i.imgur.com/hiEildI.png" width="300">
</p>

- selects rows that having matching values in two tables.

```sql
SELECT columns
FROM table1
JOIN table2
  ON table1.column1 = table2.column2
LIMIT 5;
```

here,

- `SELECT columns`: columns to show at the end of the result.
- `FROM table1`: selecting those columns from this table.
- `JOIN table2`: finding out matching values from this table.
- `ON table1.column1 = table2.column2`: to find out matching values, require to select columns from both the tables, `table1.column1` chosen column from table1, `table2.column2` chosen column from table2, `=` checks whether matching or not.
- `LIMIT 5`: limits the number of rows shown. 