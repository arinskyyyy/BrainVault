
## Operators 

All sql comparison operators can be used in a condition :
- `=` equal to
- `!=` not equal to
- `>` greater than
- `<` less than
- `>=` greater than or equal to
- `<=` less than or equal to

Like :

```sql
SELECT * 
FROM shows 
WHERE name LIKE '%the%';
```

- The `LIKE` operator can be used to search for a pattern in a column.
- this statement filters the result to only include shows with names that include 'the'.

The percentage sign `%` is a wildcard character that can be used with `LIKE`. You can use it to match characters to a pattern of your desired query.
The `%` can be used in different ways:

- `A%` matches values that begin with letter 'A'.
- `%z` matches values that end with 'z'.

Between :

```sql

```