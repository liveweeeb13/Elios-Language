# Elios Programming Language

Elios est un mini-langage de programmation conçu pour écrire des scripts de manière simple et intuitive. Ce langage supporte les fonctions personnalisées, les boucles, les conditions, les commentaires, et la gestion des erreurs. Ce fichier README explique ces fonctionnalités avec des exemples pour vous aider à démarrer.

## Table des Matières

- [Fonctions personnalisées](#1-fonctions-personnalisées)
- [Boucles (loop)](#2-boucles-loop)
- [Conditions (if/else)](#3-conditions-ifelse)
- [Commentaires](#4-commentaires)
- [Gestion des erreurs](#5-gestion-des-erreurs)
- [Utilisation](#utilisation)
- [Installation et Exécution](#installation-et-exécution)

## 1. Fonctions personnalisées

Les fonctions vous permettent de regrouper des blocs de code que vous pouvez réutiliser à plusieurs endroits dans vos scripts.

### Déclaration d'une fonction

**Syntaxe :**
```elios
§function[nomDeLaFonction] {
    !!argument!!
    §log[!!argument!!]
}
```

**Exemple :**
```elios
§function[afficherTexte] {
    !!message!!
    §log[!!message!!]
}

§call[afficherTexte, "Bonjour!"]
```
Dans cet exemple, une fonction appelée afficherTexte est définie pour afficher un message passé en argument. La fonction est ensuite appelée avec le message "Bonjour!".
