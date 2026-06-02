[← Back to projects](../README.md)

# Project 2: Log or Text Analyzer

Build a tool that reads logs or text files and produces summary statistics.

## Example Input

```text
2026-01-01 GET /users 200 23ms
2026-01-01 POST /login 500 80ms
```

## Example Output

```text
Total requests: 12000
Status 200: 10300
Status 500: 87
Top paths:
  /users 3200
  /login 900
Slowest endpoints:
  ...
```

## Learning Goals

- `File.foreach`
- Streaming file processing
- `Enumerable`
- `map`, `select`, `reduce`
- `group_by`, `tally`
- Regular expressions
- `Struct`
- Hash default values

## Completion Criteria

- Process reasonably large files without loading everything into memory.
- Keep parsing and reporting logic separate.
- Use `Enumerable` naturally instead of writing overly complex loops.
- Include sample input files and tests.
