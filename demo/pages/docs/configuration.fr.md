---
title: Configuration
weight: 20
---
# Configuration

La recherche se configure dans la section `flexsearch` de la configuration du site.

## Sections indexées

Les sections indexées sont listées sous `flexsearch.sections`, dans l’ordre des groupes de résultats. Par défaut, toutes les sections racines du site sont indexées.

### Limite

L’option `limit` définit le nombre maximum de résultats affichés dans un groupe.

### Découpage des pages

Par défaut, chaque page est découpée en un enregistrement par titre `<h2>` et `<h3>`, lié à son ancre. Utilisez `split: false` pour indexer un seul enregistrement par page, comme pour les articles de blog.

### Date

Utilisez `date: true` pour afficher la date de la page dans les résultats, à la place du fil d’Ariane.

## Options de recherche

L’option `tokenize` définit la correspondance des mots (`strict`, `forward`, `reverse` ou `full`), et `encoder` la normalisation des caractères, par exemple pour ignorer les accents.

### Poids des champs

Chaque champ indexé (titre, page, description et contenu) a une résolution, de 1 à 9 : plus elle est élevée, plus une correspondance dans ce champ est pertinente.

### Recherche approchée

Avec `suggest: true`, la recherche se rabat sur une correspondance approchée quand rien ne correspond strictement : une faute de frappe donne quand même des résultats.
