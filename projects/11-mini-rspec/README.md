[← Back to projects](../README.md)

# Project 11: Mini RSpec-like DSL

Build a tiny testing DSL inspired by RSpec.

## Example Usage

```ruby
describe Calculator do
  it "adds two numbers" do
    expect(Calculator.add(1, 2)).to eq(3)
  end
end
```

## Features

```text
describe
it
expect
eq
before
after
```

## Learning Goals

- DSL design
- Blocks
- `instance_eval`
- Method definition
- Object context
- Custom matchers
- Raising exceptions for test failures

## Completion Criteria

- Print passing and failing examples.
- Display useful failure messages.
- Support multiple examples.
- Support at least one simple matcher.
- Explain how RSpec-like DSLs are possible in Ruby.
