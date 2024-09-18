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
Dans cet exemple, une fonction appelée ``afficherTexte`` est définie pour afficher un message passé en argument. La fonction est ensuite appelée avec le message "Bonjour!".


## 2. Boucles (loop)
Les boucles permettent d'exécuter un bloc de code plusieurs fois.

### Syntaxe d'une boucle
**Syntaxe :**
```elios
§for[nombre] {
    // instructions
}
```
**Exemple :**
```§for[3] {
    §log[Itération !!index!!]
}
```

Cet exemple exécute le bloc de code 3 fois, affichant "Itération 0", "Itération 1", et "Itération 2" pour chaque itération.


## 3. ~~Conditions (if/else)~~
Les conditions permettent d'exécuter du code en fonction de la véracité d'une condition.

### Syntaxe des conditions
**Syntaxe :**
```elios
§if[condition] {
    // code si la condition est vraie
} §else {
    // code si la condition est fausse
}
```
**Exemple :**
```elios
§set[age, 25]

§if[!!age!! > 18] {
    §log[Vous êtes majeur.]
} §else {
    §log[Vous êtes mineur.]
}
```
Ici, si la variable `age` est supérieure à 18, le message "Vous êtes majeur." est affiché. Sinon, le message "Vous êtes mineur." est affiché.


## 4. Commentaires
Les commentaires permettent d'ajouter des notes dans votre code sans qu'ils soient exécutés.
## Syntaxe des commentaires
**Syntaxe :**
```elios
§comment[Ton commentaire ici]
```
**Exemple :**
```elios
§comment[Ce code affiche un message de bienvenue]
§log[Bienvenue!]
```
Dans cet exemple, le commentaire est ignoré, et seul le message "Bienvenue!" est affiché.


## 5. Gestion des erreurs
La gestion des erreurs permet de capturer et de traiter les erreurs éventuelles.
## Syntaxe de gestion des erreurs
**Syntaxe :**
```elios
§try {
    // code susceptible de provoquer une erreur
} §catch {
    // code exécuté en cas d'erreur
}
```
**Exemple :**
```elios
§try {
    §log[Tentative d'exécution...]
    // Code potentiellement dangereux ici
} §catch {
    §log[Erreur capturée !]
}
```
Le code à l'intérieur du bloc `§try` est exécuté. Si une erreur survient, le bloc  `§catch` est exécuté pour gérer l'erreur.

