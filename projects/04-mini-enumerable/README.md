[← Back to projects](../README.md)

# Project 4: Mini Enumerable Reimplementation

Reimplement a small subset of `Enumerable`.

## Methods to Implement

```text
my_map
my_select
my_reduce
my_any?
my_all?
my_find
my_group_by
my_tally
```

## Example

```ruby
module MyEnumerable
  def my_map
    result = []
    each do |item|
      result << yield(item)
    end
    result
  end
end
```

## Learning Goals

- Blocks
- `yield`
- `block_given?`
- The `Enumerable` protocol
- Why `each` is foundational
- Modules
- `include`
- Custom collections

## Completion Criteria

- Create a custom collection that only implements `each`.
- Include `MyEnumerable` to gain multiple methods.
- Test every implemented method.
- Explain why Ruby's `Enumerable` is built around `each`.
