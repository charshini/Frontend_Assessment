# Components, Services & State

## Components

- Use **standalone components** only. Do not use `NgModule` (no `@NgModule`, no feature/shared modules).
- **No inline templates.** Every component has its own external `.html` template file (`templateUrl`).
- Use **signal-based inputs and outputs** (`input()` / `output()`) instead of the `@Input()` and `@Output()` decorators.

## Services

- **One service per domain**, each in its own file.
- **No UI code or UI-related state** in service files (no view logic, no presentation/UI flags).
- All **HTTP calls** live inside services and use Angular's `HttpClient` — never the `fetch` or `XMLHttpRequest` APIs.
- **Do not swallow HTTP errors.** Catch and rethrow a clean, meaningful error instead of ignoring or silently returning.

## State Management

- Use **signals** for state management — not NgRx (or any other external state library).
- All **services** expose and manage state via signals.

## Accessibility

- Add appropriate **ARIA attributes** to all UI elements.
