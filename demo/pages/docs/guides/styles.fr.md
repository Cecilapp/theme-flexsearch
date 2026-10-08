---
title: Styles
weight: 10
---
# Styles

Les couleurs et dimensions du champ de recherche sont définies par des propriétés personnalisées CSS, avec des valeurs par défaut claires et sombres.

## Mode sombre

Le mode sombre suit la préférence du système, sauf si l’élément racine porte un attribut `data-theme`, comme le fait le sélecteur de thème de cette démo : essayez-le avec le bouton à côté du champ de recherche.

## Propriétés personnalisées

Surchargez les propriétés personnalisées dans votre propre feuille de style, par exemple pour utiliser la couleur d’accent de votre site :

```css
:root {
  --flexsearch-accent: #163c56;
  --flexsearch-selected-bg: #f2d07f;
}
```

Tous les éléments ont une classe `flexsearch-*` : les styles peuvent aussi être entièrement remplacés.
