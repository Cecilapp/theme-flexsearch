---
title: Démarrage
weight: 10
---
# Démarrage

Le thème composant _FlexSearch_ ajoute une recherche plein texte côté client à un site Cecil : l’index de recherche est généré lors du build, et interrogé dans le navigateur grâce à la bibliothèque FlexSearch. Pas de serveur, pas de service externe.

## Installation

Installez le thème avec Composer :

```bash
composer require cecil/theme-flexsearch
```

Ou téléchargez la dernière archive et décompressez son contenu dans le répertoire `themes/flexsearch`.

## Activer le thème

Ajoutez `flexsearch` dans la section `theme` de la configuration :

```yaml
theme:
  - flexsearch
```

## Ajouter le champ de recherche

Ajoutez la feuille de style dans le `<head>` du gabarit principal, puis incluez le champ de recherche à l’endroit où le bouton doit apparaître, par exemple dans l’en-tête :

```twig
{{ html(asset('flexsearch/flexsearch.css')) }}
{{ include('partials/flexsearch.html.twig') }}
```

### Déclencheur personnalisé

Tout élément portant l’attribut `data-flexsearch-open` ouvre la fenêtre de recherche, par exemple un lien du menu de navigation.
