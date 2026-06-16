# Error Handling

- Use **HTTP interceptors** to handle all errors from HTTP calls in one place.
- Interceptors **log errors** via the `LoggingService`.
- Interceptors **normalize errors** and rethrow a **clean error** to the callers.
