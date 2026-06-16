# Storage

- Create a **single `StorageService`** that encapsulates all `localStorage` and `sessionStorage` operations.
- **NEVER** access raw `localStorage` or `sessionStorage` directly from anywhere else in the code — always go through `StorageService`.
- All **error handling** related to storage lives inside `StorageService` only.
