# Logging

- **Do not use `console.xxx()` methods** (`console.log`, `console.warn`, `console.error`, etc.) scattered throughout the code.
- Create a single **`LoggingService`** exposing `log`, `warn`, `error`, `debug` (etc.) methods.
- Inject `LoggingService` wherever logging is needed; it is the only place allowed to call the underlying `console`.
