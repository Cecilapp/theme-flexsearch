---
title: Getting started
weight: 10
---
# Getting started

The _FlexSearch_ component theme adds a client side full-text search to a Cecil website: the search index is generated at build time, and searched in the browser with the FlexSearch library. No server, no external service.

## Installation

Install the theme with Composer:

```bash
composer require cecil/theme-flexsearch
```

Or download the latest archive and uncompress its contents in the `themes/flexsearch` directory.

## Enable the theme

Add `flexsearch` in the `theme` section of the configuration:

```yaml
theme:
  - flexsearch
```

## Add the search box

Add the stylesheet in the `<head>` of the main template, then include the search box where the trigger button should be displayed, for example in the header:

```twig
{{ html(asset('flexsearch/flexsearch.css')) }}
{{ include('partials/flexsearch.html.twig') }}
```

### Custom trigger

Any element with a `data-flexsearch-open` attribute opens the modal, for example a link in the navigation menu.
