[← Back to projects](../README.md)

# Project 12: Service Object and Result Pattern

Build a small business domain such as user registration or order creation.

## Example Usage

```ruby
result = RegisterUser.call(email:, password:)

if result.success?
  user = result.value
else
  puts result.error
end
```

## Learning Goals

- Small object design
- Service objects
- Result objects
- Business errors vs exceptions
- Validation
- Dependency injection
- Test doubles

## Completion Criteria

- Keep business logic independent of CLI or web frameworks.
- Represent expected failures with a `Result` object.
- Reserve exceptions for truly exceptional failures.
- Make service objects easy to test.
- Use clear error types or error objects.
