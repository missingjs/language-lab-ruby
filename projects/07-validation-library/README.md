[← Back to projects](../README.md)

# Project 7: Mini Validation Library

Build a small validation DSL inspired by Rails.

## Example Usage

```ruby
class User
  include Validatable

  attr_accessor :email, :age

  validates :email, presence: true
  validates :age, numericality: { greater_than: 0 }
end
```

## Learning Goals

- Modules
- `include`
- Class methods
- Instance methods
- Class instance variables
- DSL design
- Symbols
- `send` and `public_send`
- Basic metaprogramming

## Completion Criteria

- Support `presence` validation.
- Support `format` validation.
- Support `numericality` validation.
- Provide an `errors` object or errors collection.
- Make `valid?` return `true` or `false`.
- Include tests.
