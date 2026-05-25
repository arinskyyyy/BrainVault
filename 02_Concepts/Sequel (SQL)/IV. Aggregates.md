
## Aggregate functions 

**Aggregate functions** are used to perform calculations and return a single value.

The most common aggregate functions are :

- `COUNT()`: returns the number of rows.
- `MAX()`: returns the largest value in a column.
- `MIN()`: returns the smallest value in a column.
- `SUM()`: returns the total sum in a column.
- `AVG()`: returns the average value in a column.

`COUNT()` :

```sql
SELECT COUNT(*)
FROM table_name;
```

- the `COUNT` function counts the number of rows.

`MIN` and `MAX` :

```sql
SELECT MIN(plays)
FROM playlist;

SELECT title, artist, MAX(plays)
FROM playlist;
```

- Old & new, big & small, minimum or maximum
- `MIN` function returns the minimum of a column
- `MAX` function returns the maximum of a column

`SUM()` :

```sql
SELECT SUM(plays)
FROM playlist;
```

- The `SUM()` aggregate function takes a column and returns the total sum of the values in it.

`AVG()` :

```sql
SELECT AVG(plays)
FROM playlist;
```

- Use the `AVG()` function to calculate the average value of a column.

`GROUP BY()` :

```sql
SELECT genre, COUNT(*) 
FROM playlist 
GROUP BY genre;
```

- What this does is we are grouping together all the different `genres` and displaying two columns: the `genre`and the count of that genre.
