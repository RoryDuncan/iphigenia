# iphigenia

[![npm version](https://img.shields.io/npm/v/iphigenia.svg)](https://www.npmjs.com/package/iphigenia)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)

Bootstrap 5 utility classes with CSS custom properties using the `i-` prefix, organized in CSS layers.

## Installation

```bash
npm install iphigenia
```

## Usage

Import the CSS in your project:

```css
@import 'iphigenia';
```


Then use Bootstrap utility classes as normal:

```html
<div class="d-flex justify-content-center p-3">
  <span class="text-primary fw-bold">Hello!</span>
</div>
```

CSS custom properties use the `--i-` prefix instead of Bootstrap's default `--bs-`:

```css
.custom-element {
  color: var(--i-primary);
  padding: var(--i-spacer-3);
}
```

## Why?

- **Namespaced custom properties** — The `--i-` prefix avoids conflicts with Bootstrap's `--bs-` variables
- **CSS Layers** — Uses `@layer` for predictable cascade ordering
- **No breakpoints** — Responsive breakpoint utilities are removed for a smaller footprint

## Build

```bash
npm run build
```

Compiles `src/index.scss` to `dist/index.css`.

## License

MIT
