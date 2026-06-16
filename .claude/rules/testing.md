# Testing

Use **`TestBed`** with the **`describe` / `it`** style.

## Do

- **Unit test all smart components** (those with logic, state, and render responsibilities).
- **Unit test all services**, with appropriate mocking using Jasmine spies (`jasmine.createSpy`, `spyOn`, etc.).

## Don't / Optional

- Full unit testing of **dumb components** (render-only, no logic) **may be skipped** — a basic **smoke test** (creates successfully) is enough.
