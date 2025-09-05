# SIO-Git-Dophin
Le meilleur groupe de tous les temps. 🐬

## Pourquoi utiliser Git ? 🤔

Git est un système de gestion de versions qui permet de suivre l'évolution de ton code, de revenir en arrière si tu fais une erreur, et de collaborer efficacement avec d'autres développeurs. Il te permet de garder une trace de chaque modification faite sur ton projet, et de savoir exactement qui a changé quoi et quand. Avec Git, tu peux aussi créer des *branches* pour travailler sur des nouvelles fonctionnalités sans perturber le code principal, et plus tard, tu peux les fusionner quand elles sont prêtes. C'est super pratique quand plusieurs personnes bossent sur le même projet. En plus, Git permet de gérer les conflits de manière assez simple si deux développeurs modifient la même partie du code en même temps. Bref, Git rend le travail en équipe beaucoup plus fluide et sécurisé, et c'est devenu un standard dans le développement moderne.

## repo/commit/branche

Un dépôt (ou repository en anglais) est un espace où Git conserve tous les fichiers d'un projet ainsi que son historique. Cela inclut l'intégralité du code source et les différentes versions des fichiers à travers les commits. Un dépôt peut être local (sur ton ordinateur) ou distant (sur une plateforme comme GitHub, GitLab, etc.).

Un commit est un enregistrement d'une série de modifications dans un dépôt. Il capture l'état actuel des fichiers à un instant donné, avec un message de description. Chaque commit possède un identifiant unique, ce qui permet de retracer l'historique des changements dans le projet. Un commit te permet aussi de revenir à un état antérieur si nécessaire.

Une branche est une ligne de développement indépendante dans un dépôt Git. Elle permet de travailler sur des fonctionnalités ou corrections sans affecter la branche principale (souvent `main` ou `master`). Une branche peut être fusionnée avec d'autres branches une fois les modifications terminées.

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
