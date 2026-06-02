[← Back to projects](../README.md)

# Project 8: Mini Router DSL

Build a small routing DSL. It does not need to start a real web server.

## Example Usage

```ruby
router = Router.new do
  get "/users" do
    "list users"
  end

  post "/users" do
    "create user"
  end
end

router.call("GET", "/users")
```

## Learning Goals

- Blocks
- `instance_eval`
- DSL design
- Hash key design
- Storing and calling `Proc` objects
- Error handling

## Completion Criteria

- Support `GET` and `POST` routes.
- Return a clear result for missing routes.
- Store route handlers as blocks.
- Explain what `instance_eval` does and why it should be used carefully.
- Include tests.
