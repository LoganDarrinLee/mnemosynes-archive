*See [[Useful Stackoverflow Questions (PSQL)]] for more about serial vs integer generated as identity discussions.*

`SERIAL` [lacks integrity guarantees](https://www.naiyerasif.com/post/2024/09/04/stop-using-serial-in-postgres/). 


## Comments
#postgres/tables/comments
I didn't know you could create comments on tables and columns like this!! Awesome 

```sql

COMMENT ON TABLE users IS 'Stores user information such as name, email, and password.';

COMMENT ON TABLE users IS 'Stores user information such as name, email, and password.';

COMMENT ON COLUMN users.email IS 'The email address of the user, must be unique.';

COMMENT ON CONSTRAINT users_email_unique_constraint ON users IS 'Ensures email addresses are unique for each user.';

COMMENT ON INDEX idx_users_email IS 'Index to optimize searching by email.';

```

View comments with
```sql

-- 
SELECT obj_description(oid) FROM pg_class WHERE relname = 'table_name';


SELECT col_description('table_name'::regclass, ordinal_position) 
FROM information_schema.columns 
WHERE table_name = 'table_name';

```
### ChatGPT Breakdown
#### **When to Use Comments:**

- **Table-Level Comments**: Useful for explaining the purpose of the entire table (e.g., "Stores user data").
- **Column-Level Comments**: Useful for clarifying the purpose of specific columns (e.g., "Stores the user's date of birth").
- **Constraint/Index Comments**: Useful for explaining the reason behind constraints and indexes (e.g., "Ensures that emails are unique").
- **Other Objects**: Comments can be added to functions, views, triggers, etc., for documentation purposes.

#### **Why Use Comments:**

1. **In-Database Documentation**: These comments are stored with the database and can be viewed by anyone with the appropriate permissions, providing documentation directly in the database.
2. **Clarity for Future Developers**: They make it easier for other developers or DBAs to understand the database structure and the purpose of tables, columns, and other objects.
3. **Maintainability**: As your schema evolves, you can update comments to reflect the changes, keeping documentation up-to-date.

#### **In Summary:**

- Use the `COMMENT` command to add comments about tables and columns.
- Comments can be viewed using system catalog queries or database tools.
- This approach keeps the documentation close to the database schema, making it more accessible and useful in the long term.