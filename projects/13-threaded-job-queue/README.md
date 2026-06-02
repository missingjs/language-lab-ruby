[← Back to projects](../README.md)

# Project 13: Threaded Job Queue

Build an in-memory background job queue.

## Features

```text
enqueue job
multiple workers
failure retry
maximum retry count
graceful shutdown
```

## Learning Goals

- `Thread`
- `Queue`
- `Mutex`
- Exception handling
- Worker lifecycle
- Thread safety
- IO-bound concurrency

## Completion Criteria

- Support multiple worker threads.
- Retry failed jobs.
- Stop workers gracefully.
- Avoid losing a job that is currently running.
- Include tests.
