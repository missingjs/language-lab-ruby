[← Back to projects](../README.md)

# Project 9: Mini Gem

Package one of your small libraries as a Ruby gem.

## Good Candidates

```text
mini_config
mini_event
mini_validator
```

## Learning Goals

- RubyGems
- Bundler
- `.gemspec`
- `lib/` directory structure
- Version files
- `require`
- Semantic versioning
- README writing
- Tests and CI

## Suggested Structure

```text
mini_config/
├── lib/
│   ├── mini_config.rb
│   └── mini_config/version.rb
├── spec/
├── Gemfile
├── mini_config.gemspec
└── README.md
```

## Completion Criteria

- The gem can be required from another Ruby file.
- It has a valid gemspec.
- It has a version number.
- It has a README.
- It has tests.
- It can be built locally.
