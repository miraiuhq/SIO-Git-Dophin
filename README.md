# SIO-Git-Dophin
Le meilleur groupe de tous les temps. 🐬

## Pourquoi utiliser Git ? 🤔

Git est un système de gestion de versions qui permet de suivre l'évolution de ton code, de revenir en arrière si tu fais une erreur, et de collaborer efficacement avec d'autres développeurs. Il te permet de garder une trace de chaque modification faite sur ton projet, et de savoir exactement qui a changé quoi et quand. Avec Git, tu peux aussi créer des *branches* pour travailler sur des nouvelles fonctionnalités sans perturber le code principal, et plus tard, tu peux les fusionner quand elles sont prêtes. C'est super pratique quand plusieurs personnes bossent sur le même projet. En plus, Git permet de gérer les conflits de manière assez simple si deux développeurs modifient la même partie du code en même temps. Bref, Git rend le travail en équipe beaucoup plus fluide et sécurisé, et c'est devenu un standard dans le développement moderne.

## Table des matières
1. [Qu'est-ce que Git ?](#qu-est-ce-que-git)
2. [Initialiser un Dépôt Git](#initialiser-un-dépôt-git)
3. [Les Concepts de Base](#les-concepts-de-base)
    - Dépôt (Repo)
    - Commit
    - Branche
4. [Travailler avec Git](#travailler-avec-git)
    - Ajouter des Fichiers
    - Faire un Commit
    - Travailler avec des Branches
    - Fusionner des Branches
    - Gérer les Conflits de Fusion
5. [Collaborer avec Git](#collaborer-avec-git)
    - Cloner un Dépôt Distant
    - Pousser et Tirer (Push & Pull)
    - Résoudre les Conflits
6. [Bonnes Pratiques Git](#bonnes-pratiques-git)
    - Messages de Commit
    - Structuration des Branches
    - Gestion des Conflits
7. [Commandes Git Essentielles](#commandes-git-essentielles)

---

## Qu'est-ce que Git ?

Git est un système de gestion de versions décentralisé, permettant de suivre les changements dans un projet, d'enregistrer différentes versions et de collaborer de manière fluide entre plusieurs développeurs. Contrairement à un système centralisé, Git permet à chaque développeur d'avoir une copie complète du projet avec son historique, ce qui rend le système extrêmement rapide et fiable.

Git a été créé par Linus Torvalds en 2005 pour gérer le développement du noyau Linux. Depuis, il est devenu l'outil de contrôle de version le plus utilisé au monde.

---

## Initialiser un Dépôt Git

Pour commencer à utiliser Git, il faut initialiser un dépôt local dans ton projet. Voici comment faire :

```bash
# Se placer dans le répertoire du projet
cd /chemin/vers/ton/projet

# Initialiser un dépôt Git
git init

## Commandes Git importantes 📌

| **Commande**                            | **Description**                                                     | **Côté**         |
|-----------------------------------------|---------------------------------------------------------------------|------------------|
| `git init`                              | Initialise un nouveau dépôt Git.                                    | Client           |
| `git clone <url>`                       | Clone un dépôt distant sur votre machine locale.                    | Client           |
| `git status`                            | Affiche l'état des fichiers dans le dépôt (modifié, non suivi, etc.).| Client           |
| `git add <file>`                        | Ajoute un fichier au "staging area" avant le commit.                | Client           |
| `git commit -m "message"`               | Crée un commit avec un message descriptif.                          | Client           |
| `git log`                               | Affiche l'historique des commits.                                   | Client           |
| `git diff`                              | Affiche les différences entre les fichiers modifiés et le dernier commit. | Client        |
| `git branch`                            | Affiche la liste des branches locales, ou crée une nouvelle branche. | Client         |
| `git checkout <branch>`                 | Bascule vers une autre branche.                                     | Client           |
| `git merge <branch>`                    | Fusionne une branche avec la branche active.                        | Client           |
| `git pull`                              | Récupère et fusionne les modifications du dépôt distant.            | Client / Serveur |
| `git push`                              | Envoie les commits locaux vers le dépôt distant.                    | Client / Serveur |
| `git remote add <name> <url>`           | Ajoute un dépôt distant au projet local.                            | Client           |
| `git reset <commit>`                    | Annule un ou plusieurs commits.                                     | Client           |
| `git fetch`                             | Récupère les modifications du dépôt distant sans les appliquer.    | Serveur          |
| `git push --force`                      | Force l'envoi des commits locaux sur le dépôt distant (attention à l'écrasement). | Serveur |
| `git pull --rebase`                     | Récupère et réapplique les commits locaux sur la branche mise à jour. | Serveur         |
| `git tag`                               | Crée un tag pour marquer un point spécifique dans l'historique.     | Client / Serveur |
| `git branch -r`                         | Affiche les branches distantes.                                     | Serveur          |
| `git cherry-pick <commit>`              | Applique un commit spécifique d'une branche à une autre.            | Client / Serveur |
| `git stash`                             | Met de côté les modifications non committées pour revenir à un état propre. | Client     |
| `git rebase`                            | Réécrit l'historique des commits, souvent utilisé pour mettre à jour une branche. | Client |
