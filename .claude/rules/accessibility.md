# Accessibility

- Comply with **WCAG 2.1 Level AA** wherever applicable when building HTML elements.

## Key considerations

- **Semantic HTML** — use the correct elements (`button`, `nav`, `main`, `header`, `footer`, headings in order) before reaching for ARIA.
- **ARIA attributes** — add appropriate roles/labels on UI elements where semantics alone are insufficient.
- **Keyboard accessibility** — all interactive elements must be reachable and operable via keyboard, with a visible focus indicator.
- **Color contrast** — meet AA contrast ratios (4.5:1 for normal text, 3:1 for large text and UI/graphical elements).
- **Text alternatives** — meaningful `alt` text for images; labels for form controls.
- **Forms** — associate labels with inputs, group related fields, and surface clear, programmatically linked error messages.
- **Resize & reflow** — content remains usable at 200% zoom without loss of functionality.
