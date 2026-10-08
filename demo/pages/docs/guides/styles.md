---
title: Styles
weight: 10
---
# Styles

Colors and sizes of the search box are defined as CSS custom properties, with light and dark defaults.

## Dark mode

The dark mode follows the system preference, unless the root element has a `data-theme` attribute, as set by the theme selector of this demo: try it with the button next to the search box.

## Custom properties

Override the custom properties in your own stylesheet, for example to use the accent color of your website:

```css
:root {
  --flexsearch-accent: #163c56;
  --flexsearch-selected-bg: #f2d07f;
}
```

All elements have a `flexsearch-*` class, so the styles can also be fully replaced.
