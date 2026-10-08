---
title: Traductions
weight: 20
---
# Traductions

Le champ de recherche est traduit en anglais et en français, et un index est généré pour chaque langue du site : passez en anglais avec le lien du pied de page, la recherche ne renvoie alors que les pages anglaises.

## Ajouter une langue

Extrayez les chaînes à traduire dans une autre langue avec la commande suivante, puis traduisez le fichier généré :

```bash
cecil util:translations:extract --locale=<locale> --save --theme=flexsearch
```
