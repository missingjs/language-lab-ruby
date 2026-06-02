[← Back to projects](../README.md)

# Project 5: Mini Event System

Build a simple event system.

## Example Usage

```ruby
events.on(:user_created) do |user|
  puts "new user: #{user.email}"
end

events.emit(:user_created, user)
```

## Features

```text
on
off
once
emit
listener_count
```

## Learning Goals

- Blocks as callbacks
- `Proc`
- `lambda`
- Hashes of arrays
- Symbols
- Object responsibility
- Error handling

## Possible Extension

```ruby
events.around(:user_created) do |event|
  puts "before"
  event.call
  puts "after"
end
```

## Completion Criteria

- Register and remove listeners.
- Support one-time listeners.
- Store blocks as `Proc` objects.
- Use symbols as event names.
- Include tests.
