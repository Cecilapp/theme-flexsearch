---
title: Translations
weight: 20
---
# Translations

The search box is translated in English and French, and an index is generated for each language of the website: switch to French with the link in the footer, the search only returns French pages.

## Add a language

Extract the strings to translate in another language with the following command, then translate the generated file:

```bash
cecil util:translations:extract --locale=<locale> --save --theme=flexsearch
```
