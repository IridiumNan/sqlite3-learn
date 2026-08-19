# sqlite learn note

[official docs](https://sqlite.org/cli.html)

## DOT COMMANDS

```sql
.tables -- show tables
.save <file name> -- save changee
.open <file name> -- reopen or open a database
.quit -- exit the sqlite3
```

## CREATE

```sql
CREATE TABLE coffee_table (
    id INT PRIMARY KEY,
    name TEXT,
    region TEXT,
    roast TEXT
);
```

---

## INSERT

```sql
INSERT INTO coffee_table (id, name, region, roast)
VALUES (1, 'default route', 'ethiopia', 'light');
```

> [!NOTE]
> Use the ' instead of "

---

## SELECT

```sql
SELECT id, name FROM coffee_table;

-- select with condition
SELECT id, name FROM coffee_table 
WHERE id = 1;
```

---

## UPDATE

```sql
UPDATE coffee_table SET name = NULL where id = 1;
```

---

## DELETE

```sql
DELETE FROM coffee_table
WHERE id = 1;
```
