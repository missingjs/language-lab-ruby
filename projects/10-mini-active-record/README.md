[← Back to projects](../README.md)

# Project 10: Mini Active Record Pattern

Build a very small ORM-style data access layer without Rails. Start with SQLite.

## Example Usage

```ruby
user = User.find(1)
users = User.where(email: "a@example.com")
user.save
```

## Learning Goals

- `sqlite3` gem
- Class methods
- Instance methods
- Object mapping
- Careful use of dynamic dispatch
- SQL basics
- Error handling

## Scope

Keep the scope small. Support only:

```text
find
where
save
delete
```

## Completion Criteria

- Map database rows to Ruby objects.
- Save objects to the database.
- Use parameterized SQL rather than unsafe string interpolation.
- Use a test database.
- Explain why a complete ORM is much more complex than this project.
