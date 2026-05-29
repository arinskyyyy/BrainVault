## Left Join

`LEFT JOIN OR LEFT OUTER JOIN`:

<p align="center">
  <img src="https://i.imgur.com/mqeWbEj.png" width="300">
</p>

- `LEFT JOIN` will keep all the rows from the left table, plus matched rows in the right table.

```sql
SELECT columns
FROM table1
LEFT JOIN table2
  ON table1.column1 = table2.column2;
```

Difference between `JOIN` and `LEFT JOIN`:

`JOIN`:
- Returns rows where there’s a match in both tables.
- If there’s no match, that row is excluded.

`LEFT JOIN`:
- Returns all rows from the left table, and matched rows from the right.
- If there’s no match on the right, you’ll still get the left row... but with `NULL`s for the right-side columns.

`UNION`:

- another simple way to combine two tables, without duplicates.

```sql
SELECT columns
FROM table1
UNION
SELECT columns
FROM table2;
```

