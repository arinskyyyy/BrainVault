
## Comparison Operators

All sql comparison operators can be used in a condition :
- `=` equal to
- `!=` not equal to
- `>` greater than
- `<` less than
- `>=` greater than or equal to
- `<=` less than or equal to

LIKE :

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

BETWEEN :

```sql
SELECT *
FROM shows
WHERE name
BETWEEN 'A' AND 'D';
```

- The `BETWEEN` operator is used in a `WHERE` clause to filter the result set within a certain range (inclusively for the numeric BETWEEN).
-  The range must be separated by an `AND` keyword.

Using BETWEEN with numbers :

- **What it means:** `BETWEEN 2020 AND 2025` tells the database to find all records where the year is 2020, 2021, 2022, 2023, 2024, or 2025.
- **Key takeaway:** Number ranges are **inclusive**. The start value (2020) and the end value (2025) are both included in the final results.

Using `BETWEEN` with Text (Alphabetical Filtering) :

- **What it means:** `BETWEEN 'A' AND 'D'` tells the database to find everything that starts with A, B, or C.
- **The Tricky Part (The Note):** You might expect this range to include words that start with D, like "Dragon Ball Super", but it does not. Here is why:
    
    - In alphabetical sorting, the exact single letter **'D'** comes before **'Da'**, **'Do'**, or **'Dr'**.
    - Because the range explicitly ends at the exact character **'D'**, anything with additional letters after the 'D' (like "Dragon") is mathematically considered _greater_ than 'D' and falls outside the range.
    - The only way a title starting with 'D' would be returned is if the entire title was literally just the single letter **'D'**.

**In short:** If you want to include all shows that start with the letter D in your results, using `BETWEEN 'A' AND 'D'` will not work. You would instead need to use a range like `BETWEEN 'A' AND 'E'` or use the `LIKE` operator.

**In simple words :** using `BETWEEN 'A' AND 'D'` will result in giving words which starts with A, B, C and D, however, it will only include words which are exactly 'D' excluding other words which consists 'Da', 'Do' or 'Dragon' anything, why? because these words are greater than 'D' to include these words, require to increase the range, from 'D' to 'E', now it cover the words between 'D' to 'E'.