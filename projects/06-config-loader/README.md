[← Back to projects](../README.md)

# Project 6: Configuration Loader

Build a configuration loader.

## Supported Inputs

```text
config.yml
config.json
environment variable overrides
default values
required field validation
```

## Example Usage

```ruby
config = Config.load("config.yml")
config.database_url
config.port
```

## Learning Goals

- YAML and JSON parsing
- Hashes
- Symbol keys vs string keys
- `fetch` and `dig`
- The tradeoffs of `OpenStruct`
- Custom error classes
- Object API design

## Completion Criteria

- Report clear errors for missing configuration.
- Support defaults.
- Support `ENV` overrides.
- Avoid leaking internal hashes unnecessarily.
- Include tests.
