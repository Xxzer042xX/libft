# Libft

Libft est une bibliothèque C standard que j'ai développée pour fournir des fonctions utilitaires communes et souvent utilisées en programmation C. Elle comprend des fonctions pour la manipulation de chaînes, la gestion de la mémoire, et des fonctionnalités bonus liées aux listes chaînées.

## Table des Matières

- [Introduction](#introduction)
- [Fonctionnalités](#fonctionnalités)
- [Installation](#installation)
- [Utilisation](#utilisation)
- [Exemples](#exemples)
- [Contribuer](#contribuer)
- [Licence](#licence)

## Introduction

Libft est conçue pour offrir des fonctions similaires à celles trouvées dans les bibliothèques standard de C. Elle est particulièrement utile pour les projets où vous avez besoin de fonctionnalités de base sans dépendre de la bibliothèque standard C.

## Fonctionnalités

### Fonctions de Manipulation de Chaînes

- `ft_strlen` - Retourne la longueur d'une chaîne.
- `ft_strchr` - Trouve la première occurrence d'un caractère dans une chaîne.
- `ft_strcmp` - Compare deux chaînes de caractères.

### Fonctions de Gestion de la Mémoire

- `ft_memset` - Remplit un bloc de mémoire avec une valeur donnée.
- `ft_calloc` - Alloue et initialise une zone de mémoire.
- `ft_strdup` - Duplique une chaîne de caractères.

### Fonctions Bonus (Listes Chaînées)

- `ft_lstnew` - Crée un nouvel élément de liste.
- `ft_lstadd_front` - Ajoute un élément au début de la liste.
- `ft_lstsize` - Compte le nombre d'éléments dans la liste.

## Installation

Pour compiler et utiliser Libft, suivez ces étapes :

1. **Clonez le dépôt :**

   ```bash
   git clone https://github.com/votre-utilisateur/votre-repo.git
   ```

2. **Accédez au répertoire du projet :**

   ```bash
   cd votre-repo
   ```

3. **Compilez la bibliothèque :**

   ```bash
   make
   ```

   Cette commande générera le fichier `libft.a` dans le répertoire racine du projet.

## Utilisation

Pour utiliser Libft dans votre projet, ajoutez le fichier d'en-tête `libft.h` et liez la bibliothèque `libft.a` lors de la compilation de votre projet. Voici un exemple de compilation :

```bash
gcc -o mon_programme mon_programme.c -L. -lft
```

Assurez-vous d'inclure le répertoire `include` dans les chemins de recherche des en-têtes, si vous avez choisi de stocker vos fichiers d'en-tête dans un répertoire `include`.

## Exemples

Voici quelques exemples d'utilisation des fonctions principales de Libft :

```c
#include "libft.h"
#include <stdio.h>

int main(void) {
    char str[] = "Hello, World!";
    printf("La longueur de la chaîne est : %zu\n", ft_strlen(str));
    printf("Première occurrence de 'W': %s\n", ft_strchr(str, 'W'));
    return 0;
}
```

## Contribuer

Si vous souhaitez contribuer à Libft, vous pouvez :

1. **Faire une demande de fusion (Pull Request)** en ajoutant vos modifications ou améliorations.
2. **Signaler des problèmes** en ouvrant une issue sur le dépôt GitHub.
3. **Discuter des améliorations potentielles** en ouvrant une issue ou en soumettant des propositions.

Veuillez vous assurer de tester vos contributions et de respecter les bonnes pratiques de codage.

## Licence

Ce projet est sous la licence [MIT](LICENSE).
