# Création et publication d'un projet C sur GitHub

## Objectif

Apprendre à créer un projet C basique en utilisant le terminal et à le publier sur GitHub. Cet exercice combinera les compétences terminales acquises avec les bases de Git pour partager votre code.

## Commandes à Apprendre

- Toutes les commandes des exercices précédents
- `git init` - Initialiser un dépôt Git
- `git add` - Ajouter des fichiers à l'index
- `git commit` - Enregistrer les modifications
- `git remote` - Gérer les dépôts distants
- `git push` - Envoyer les modifications vers un dépôt distant
- `gcc` - Compiler des fichiers C

## Prérequis

- Un compte GitHub (créez-en un si vous n'en avez pas)
- Git installé sur votre machine
- GCC installé sur votre machine

## Exercice

### Partie 1: Création du projet C

1. Créez un dossier de projet appelé "hello_github" et un sous-dossier "src" en utilisant uniquement les commandes du terminal:

   ```
   hello_github/
   └── src/
   ```

2. Créez les fichiers suivants:

   - `src/main.c` avec un programme simple qui affiche "Hello, GitHub!"
   - `.gitignore` qui ignore les fichiers compilés (.o, exécutables)

3. Dans le fichier `src/main.c`, écrivez un programme simple qui affiche "Hello, GitHub!" à l'écran. Voici le code à utiliser:

   ```c
   /*
    * main.c
    * Programme simple qui affiche "Hello, GitHub!"
    */

   #include <stdio.h>

   int main(void) {
       printf("Hello, GitHub!\n");
       return 0;
   }
   ```

4. Compilez votre programme en utilisant gcc avec la commande:

   ```
   gcc src/main.c -o hello_github
   ```

5. Exécutez votre programme pour vérifier qu'il fonctionne correctement

### Partie 2: Publication sur GitHub

1. Initialisez un dépôt Git dans votre dossier de projet
2. Ajoutez tous vos fichiers à l'index Git
3. Effectuez votre premier commit avec un message descriptif
4. Créez un nouveau dépôt public sur GitHub appelé "hello_github"
5. Connectez votre dépôt local au dépôt distant
6. Poussez votre code vers GitHub

### Partie 3: Documentation

Créez un fichier `git_commands_log.txt` qui documente:

1. Toutes les commandes Git que vous avez utilisées, dans l'ordre
2. Une explication brève de ce que fait chaque commande

## Résultat attendu

- Un dépôt GitHub public contenant votre projet C "hello_github"
- Un programme C fonctionnel qui affiche "Hello, GitHub!" lorsqu'il est exécuté
- Une documentation complète des commandes Git utilisées

## Conseils

- Assurez-vous de configurer Git avec votre nom et email avant de faire un commit:
  ```
  git config --global user.name "Votre Nom"
  git config --global user.email "votre.email@exemple.com"
  ```
- Utilisez `git status` fréquemment pour voir l'état de votre dépôt
- Pour créer un nouveau dépôt sur GitHub, vous devrez vous connecter à votre compte et cliquer sur le bouton "New repository"
- Pour la connexion à GitHub, vous pouvez utiliser HTTPS ou SSH (SSH est recommandé pour un usage régulier)
