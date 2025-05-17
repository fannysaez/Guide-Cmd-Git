
# 30 commandes Git utiles à connaître pour mieux gérer ton code

<div align="center">
  <img src="./assets/svg/git-commands-logo.svg" alt="Git 30 commandes utiles" width="500">
</div>

---

> Quand on commence à utiliser Git, on se limite souvent à git add, git commit, et git push...
> Mais Git propose bien plus pour suivre, tester, corriger ou organiser son travail au quotidien.

Voici une sélection de 30 commandes que je trouve pratiques :

## 📋 Table des matières

- [1. Démarrer avec Git](#1-démarrer-avec-git)
- [2. Suivre les changements](#2-suivre-les-changements)
- [3. Travailler avec des branches](#3-travailler-avec-des-branches)
- [4. Travailler avec un dépôt distant](#4-travailler-avec-un-dépôt-distant-ex--github)
- [5. Consulter l'historique et les changements](#5-consulter-lhistorique-et-les-changements)
- [6. Annuler, restaurer ou mettre de côté](#6-annuler-restaurer-ou-mettre-de-côté)
- [7. Pour aller plus loin](#7-pour-aller-plus-loin)

---

## 1. Démarrer avec Git

| Commande | Description |
|----------|-------------|
| `git init` | Crée un dépôt Git vide dans le dossier actuel (pour commencer à versionner un projet). |
| `git clone [url]` | Récupère un projet depuis un dépôt en ligne (GitHub, GitLab...) et le copie sur votre machine. |
| `git config --global user.name "TonNom"` | Définit ton nom d'auteur pour tous les projets. |
| `git config --global user.email "email@example.com"` | Idem pour l'adresse email associée aux commits. |

## 2. Suivre les changements

| Commande | Description |
|----------|-------------|
| `git status` | Affiche les fichiers modifiés, ajoutés ou supprimés. |
| `git add [fichier]` | Prépare un fichier pour le commit (le place dans la "staging area"). |
| `git add .` | Ajoute tous les fichiers modifiés à la staging area. |
| `git commit -m "Message"` | Enregistre officiellement les modifications avec un message descriptif. |
| `git commit --amend` | Modifie le dernier commit (pour corriger un oubli ou un message). |

## 3. Travailler avec des branches

| Commande | Description |
|----------|-------------|
| `git branch` | Affiche la liste des branches existantes. |
| `git branch nom_branche` | Crée une nouvelle branche. |
| `git checkout nom_branche` | Change de branche. |
| `git checkout -b nom_branche` | Crée une branche ET bascule dessus directement. |
| `git merge nom_branche` | Fusionne une branche dans celle en cours. |
| `git branch -d nom_branche` | Supprime une branche locale. |

## 4. Travailler avec un dépôt distant (ex : GitHub)

| Commande | Description |
|----------|-------------|
| `git remote -v` | Liste les dépôts distants (pour voir si ton projet est lié à GitHub). |
| `git remote add origin [url]` | Connecte ton dépôt local à un dépôt distant. |
| `git push origin branche` | Envoie ton code vers le dépôt distant. |
| `git pull origin branche` | Récupère et fusionne les modifs du dépôt distant. |
| `git fetch origin` | Récupère les modifs du dépôt sans les fusionner automatiquement. |

## 5. Consulter l'historique et les changements

| Commande | Description |
|----------|-------------|
| `git log` | Liste tous les commits effectués. |
| `git log --oneline` | Affiche les commits en version compacte. |
| `git diff` | Montre les différences non ajoutées (entre fichier modifié et version enregistrée). |
| `git diff --staged` | Montre les différences déjà ajoutées (en attente de commit). |

## 6. Annuler, restaurer ou mettre de côté

| Commande | Description |
|----------|-------------|
| `git reset fichier` | Enlève un fichier de la staging area (mais garde les modifs). |
| `git reset --hard [commit]` | Repart sur un ancien commit et supprime tout ce qu'il y a après. |
| `git stash` | Sauvegarde temporairement les modifs en cours (pour changer de branche sans perdre). |
| `git stash pop` | Récupère les modifications mises de côté. |

## 7. Pour aller plus loin

| Commande | Description |
|----------|-------------|
| `git rebase branche` | Rejoue les commits d'une branche sur une autre, pour un historique plus propre. |
| `git cherry-pick [commit]` | Applique un commit précis sur ta branche actuelle (sans tout fusionner). |

---

<div align="center">
  
## 💡 Astuces supplémentaires

</div>

- Crée des **alias Git** pour accélérer tes commandes fréquentes:
  ```bash
  git config --global alias.co checkout
  git config --global alias.br branch
  git config --global alias.ci commit
  git config --global alias.st status
  ```

<!-- - Utilise un **outil graphique** comme GitKraken, SourceTree ou l'intégration Git de ton IDE pour visualiser plus facilement les branches.

- Envisage d'utiliser un fichier `.gitignore` pour exclure automatiquement certains fichiers du versionnement (logs, fichiers de config, dossiers de dépendances...). -->

---

<div align="center">
  
*Enregistre ce fichier comme mémo personnel ou partage-le avec ton équipe pour vous aider à mieux exploiter Git !*

[![Licence MIT](https://img.shields.io/badge/Licence-MIT-blue.svg)](LICENSE)

</div>
