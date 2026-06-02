# Project-Based Learning Path

The goal is not to rush into Rails immediately, but to build a strong foundation in Ruby itself: objects, blocks, Enumerable, modules, testing, gems, metaprogramming, DSL design, and the Ruby mechanisms behind Rails and RSpec.

## Core Approach

Ruby is a highly expressive object-oriented language with strong support for blocks, dynamic dispatch, mixins, DSLs, and metaprogramming. A good Ruby project roadmap should gradually move through these layers:

```text
Ruby core
→ Enumerable and data transformation
→ object-oriented design
→ blocks and callbacks
→ testing and gems
→ DSL and metaprogramming
→ Rails-like mechanisms
→ concurrency and performance
```

Each project should focus on a small number of learning goals. Do not try to build a full Rails application too early. Rails is powerful, but it hides many Ruby mechanisms that are worth learning directly first.

For the conceptual map behind these projects, see [../roadmap.md](../roadmap.md).

---

## The Fifteen Projects

1. [CLI TODO Tool](01-cli-todo/README.md) — Ruby syntax, classes, file I/O, JSON persistence, basic testing.
2. [Log or Text Analyzer](02-text-analyzer/README.md) — `File.foreach`, Enumerable, regex, streaming.
3. [CSV Expense Tracker](03-csv-expense-tracker/README.md) — CSV stdlib, `BigDecimal`, hash aggregation, Date/Time.
4. [Mini Enumerable Reimplementation](04-mini-enumerable/README.md) — Blocks, `yield`, modules, the `each` protocol.
5. [Mini Event System](05-mini-event-system/README.md) — Procs as callbacks, `lambda`, hashes of arrays.
6. [Configuration Loader](06-config-loader/README.md) — YAML/JSON parsing, `fetch`/`dig`, custom errors.
7. [Mini Validation Library](07-validation-library/README.md) — Modules, class methods, basic metaprogramming, DSL design.
8. [Mini Router DSL](08-router-dsl/README.md) — Blocks, `instance_eval`, storing Procs, DSL design.
9. [Mini Gem](09-mini-gem/README.md) — RubyGems, Bundler, `.gemspec`, semantic versioning.
10. [Mini Active Record Pattern](10-mini-active-record/README.md) — `sqlite3`, class/instance methods, parameterized SQL.
11. [Mini RSpec-like DSL](11-mini-rspec/README.md) — DSL design, `instance_eval`, custom matchers.
12. [Service Object and Result Pattern](12-service-object/README.md) — Service objects, Result objects, dependency injection.
13. [Threaded Job Queue](13-threaded-job-queue/README.md) — `Thread`, `Queue`, `Mutex`, worker lifecycle.
14. [Fiber-based Task Scheduler](14-fiber-scheduler/README.md) — `Fiber`, cooperative concurrency, scheduler concepts.
15. [Performance Profiling Lab](15-performance-lab/README.md) — `Benchmark`, `memory_profiler`, `stackprof`, allocation reduction.

---

## Recommended Project Order

```text
1. CLI TODO Tool
2. Log or Text Analyzer
3. CSV Expense Tracker
4. Mini Enumerable Reimplementation
5. Mini Event System
6. Configuration Loader
7. Mini Validation Library
8. Mini Router DSL
9. Mini Gem
10. Mini Active Record Pattern
11. Mini RSpec-like DSL
12. Service Object and Result Pattern
13. Threaded Job Queue
14. Fiber-based Task Scheduler
15. Performance Profiling Lab
```

This sequence moves through:

```text
Ruby syntax and objects
→ standard library and data transformation
→ blocks and Enumerable
→ Proc and event callbacks
→ configuration and object API design
→ DSL and metaprogramming
→ gem packaging
→ Rails-like internals
→ testing DSLs
→ application service design
→ concurrency
→ performance
```

---

## If Time Is Limited

The most important projects are:

```text
1. Log or Text Analyzer
2. Mini Enumerable Reimplementation
3. Mini Event System
4. Mini Validation Library
5. Mini Router DSL
6. Mini Gem
7. Mini RSpec-like DSL
```

These cover the Ruby skills that matter most:

```text
Enumerable
blocks
Proc
modules
mixins
DSLs
metaprogramming
object model
testing culture
gem engineering
```

If you also want a stronger backend engineering path, add:

```text
8. Service Object and Result Pattern
9. Threaded Job Queue
```

---

## Suggested Three-Version Workflow

For each project, use three passes.

### Version 1: Make It Work

Focus on functionality first.

Priorities:

- Clear object responsibilities
- Short methods
- Working tests
- Basic error handling

### Version 2: Make It Ruby-like

Refactor toward idiomatic Ruby.

Priorities:

- `Enumerable`
- Blocks
- Symbols
- Keyword arguments
- Small objects
- Natural method names
- Custom errors

### Version 3: Add Ruby Power Carefully

Only then add more dynamic Ruby features.

Possible techniques:

- DSLs
- Module inclusion
- `define_method`
- `public_send`
- `instance_eval`
- `method_missing`

Always ask whether the metaprogramming makes the code clearer or only more clever.

---

## Skill Levels by Project Cluster

The Stage One through Stage Seven structure in [../roadmap.md](../roadmap.md) describes the **knowledge map**. The clusters below describe what skills you should have practiced after finishing the corresponding **projects**.

### Beginner Level: Projects 1 to 3

You should become comfortable with:

- Ruby syntax
- Strings, symbols, arrays, and hashes
- File, JSON, and CSV handling
- Classes and objects
- Basic error handling
- Minitest or RSpec
- Bundler basics

### Intermediate Level: Projects 4 to 9

You should become comfortable with:

- Blocks
- `yield`
- `Proc` and `lambda`
- `Enumerable`
- Modules
- `include` and `extend`
- DSL design
- Bundler and gemspecs
- Test organization

### Advanced Level: Projects 10 to 15

You should become comfortable with:

- Ruby object model
- Method lookup
- Metaprogramming
- Rails-like DSLs
- RSpec-like DSLs
- Service objects
- Threads and fibers
- Profiling and performance tuning

---

## Projects to Avoid Too Early

These are useful later, but not ideal early language-learning projects:

```text
Full Rails SaaS application
Complex e-commerce system
Large GraphQL API
Complete ORM
Complete testing framework
Complex background job system
Large metaprogramming DSL
High-concurrency web server
```

They combine too many concerns at once:

```text
Rails
databases
deployment
authentication
authorization
caching
queues
frontend code
testing
metaprogramming
performance
```

Early projects should be small and focused.

---

## Questions to Ask While Building

For each project, ask:

```text
Is this object's responsibility clear?
Does this method name feel natural in Ruby?
Would a block make this API clearer?
Can Enumerable simplify this logic?
Should this failure raise an exception or return a Result?
Is this module a namespace or a mixin?
Am I using include, extend, or prepend correctly?
Does this DSL improve readability?
Is this metaprogramming worth the cost?
Can this monkey patch be avoided?
Do the tests describe behavior clearly?
```

---

## Advanced Ruby Practitioner Goals

After completing this project roadmap, you should be able to write Ruby code that is:

```text
clear in object responsibility
natural in Enumerable usage
solid in blocks, Proc, and lambda
careful with modules and mixins
explicit in error handling
well tested
comfortable with Bundler and gems
moderate in DSL design
restrained in metaprogramming
readable in Rails and RSpec internals
aware of Ruby concurrency and performance boundaries
```

The goal is not to rush into Rails. The goal is to understand why Ruby makes Rails, RSpec, Rake, and other DSL-heavy tools possible. Once you understand objects, blocks, Enumerable, modules, and metaprogramming, Rails will feel much less magical and much more Ruby-like.
