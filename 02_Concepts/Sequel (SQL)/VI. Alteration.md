
**Alter Table**

`ALTER TABLE/ ADD COLUMN` statement adds a new column to an existing table.

```sql
ALTER TABLE companies
ADD COLUMN about TEXT;
```

- This statement adds a new `TEXT` column called `about` to the `companies` table.

`UPDATE SET` :

- Mistakes and outdated data happens, which means we need to go in and update some values in the table
- The `UPDATE` statement edits a row in a table.
- Elon Musk changed Twitter’s name to X in 2023, let’s update the name:

```sql
UPDATE companies
SET name = 'X'
WHERE name = 'Twitter';
```

`DELETE FROM` :

```sql
DELETE FROM companies
WHERE name = 'BeReal';
```

- `DELETE FROM` statement removes one or more rows from a table.
- Here, we are deleting the whole row(s) `WHERE name = 'BeReal';`