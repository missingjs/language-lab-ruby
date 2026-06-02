[← Back to projects](../README.md)

# Project 1: CLI TODO Tool

Build a command-line TODO application.

## Example Commands

```text
todo add "learn Ruby"
todo list
todo done 1
todo remove 1
todo search ruby
```

## Learning Goals

- Ruby syntax
- Strings and symbols
- Arrays and hashes
- Method definitions
- Classes and objects
- File I/O
- JSON persistence
- Basic error handling
- Minitest or RSpec
- Bundler basics

## Suggested Structure

```text
ruby-todo/
├── lib/
│   ├── todo.rb
│   ├── todo/task.rb
│   ├── todo/store.rb
│   └── todo/cli.rb
├── spec/
├── Gemfile
└── README.md
```

## Completion Criteria

- Add, list, complete, remove, and search tasks.
- Persist data to a local JSON file.
- Separate domain logic from CLI parsing.
- Avoid putting all logic in a single `main.rb` file.
- Include tests for core behavior.
