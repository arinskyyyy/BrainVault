
ORDER BY :

```sql
SELECT name, genre, stream, year
FROM shows
ORDER BY year;
```

- the `ORDER BY` statement sorts rows of data in ascending or descending order.
- by default, this command sorts the data into ascending order.

In descending order : 

```sql
SELECT name, genre, stream, year
FROM shows
ORDER BY year DESC;
```

- `DESC` command is used to sort data in descending order.

IN and OR :

```sql
SELECT *
FROM restaurant
WHERE cuisine IN ('Chinese', 'Italian');
```

- to find whether the 'Chinese' or 'Italian' food is in cuisine use `IN`.
- `OR` can be used, however, one would have to write similar to block mentioned below: 

```sql
SELECT *
FROM restaurant
WHERE cuisine = 'Chinese' OR cuisine = 'Italian';
```
