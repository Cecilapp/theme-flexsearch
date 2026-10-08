---
title: Configuration
weight: 20
---
# Configuration

The search is configured in the `flexsearch` section of the website configuration.

## Indexed sections

The indexed sections are listed under `flexsearch.sections`, in the order of the result groups. By default, every root section of the website is indexed.

### Limit

The `limit` option sets the maximum number of results displayed in a group.

### Split pages

By default, each page is split into one record per `<h2>` and `<h3>` heading, linked to its anchor. Set `split: false` to index a single record per page, as for blog posts.

### Date

Set `date: true` to display the date of the page in the results, instead of the breadcrumb.

## Search options

The `tokenize` option sets how words are matched (`strict`, `forward`, `reverse` or `full`), and `encoder` sets how characters are normalized, for example to ignore accents.

### Fields weight

Each indexed field (title, page, description and content) has a resolution, from 1 to 9: the higher, the more relevant a match in this field.

### Fuzzy matching

With `suggest: true`, the search falls back to fuzzy matching when nothing matches strictly, so a typo still returns results.
