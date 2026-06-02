[← Back to projects](../README.md)

# Project 3: CSV Expense Tracker

Build a CSV-based expense tracking tool.

## Example Commands

```text
expense add --amount 12.5 --category food --note lunch
expense list
expense summary --by category
expense summary --month 2026-06
```

## Learning Goals

- Ruby CSV standard library
- `Date` and `Time`
- `BigDecimal`
- Hash aggregation
- Object modeling
- Command-line arguments
- Input validation and error handling

## Suggested Model

```ruby
Expense = Struct.new(:amount, :category, :date, :note, keyword_init: true)
```

or:

```ruby
class Expense
  attr_reader :amount, :category, :date, :note
end
```

## Completion Criteria

- Avoid using `Float` carelessly for money.
- Support summaries by category and month.
- Read and write CSV clearly.
- Provide friendly errors for invalid input.
- Include tests.
