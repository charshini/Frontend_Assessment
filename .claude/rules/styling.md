# Styling & Theming

- Use **SCSS** for theming.
- Split the theming layers across **separate files**: primitives, semantic combinations, and themes.
- A **`ThemeService`** owns the responsibility of toggling between themes.

## Layers

### 1. Primitives (stored separately)

Raw design tokens — colors, spacing, etc. No semantic meaning.

```scss
--primary--blue: #324324;
--primary--green: #DE4324;
```

### 2. Semantic combinations (light theme = default)

Map primitives to meaningful, usage-based variables. The light theme is the default.

```scss
--header-background: var(--primary--blue);
--footer-background: var(--primary--green);
```

### 3. Themes (actual theme overrides)

Override semantic variables per theme.

```scss
.dark-theme {
  --header-background: var(--dark-blue);
}
```

## ThemeService

- Handles the **toggle operation** of switching between light and dark themes.
- Applies the active theme (`light` | `dark`) to the **`body` element**.
