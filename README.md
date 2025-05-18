
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
### 🗂️ Structure des 30 commandes Git

```bash
📂 30 Commands Git
│── 📄 README.md         --> Page d'accueil avec introduction et table des matières
│── 📄 getting-started.md   --> Démarrer avec Git (Section 1)
│── 📄 tracking-changes.md  --> Suivre les changements (Section 2)
│── 📄 working-with-branches.md  --> Travailler avec des branches (Section 3)
│── 📄 remote-repositories.md    --> Travailler avec un dépôt distant (Section 4)
│── 📄 history-and-changes.md    --> Consulter l'historique et les changements (Section 5)
│── 📄 undo-and-restore.md       --> Annuler, restaurer ou mettre de côté (Section 6)
│── 📄 advanced-commands.md      --> Pour aller plus loin (Section 7)
│── 📄 git-aliases.md           --> Astuces et alias Git
│── 📂 assets                   --> Dossier pour les ressources
│   ├── 📄 git-commands-logo.svg    --> Logo principal
│   ├── 🖼️ git-workflow.png         --> Schéma du workflow Git
│   ├── 🖼️ branch-example.png       --> Illustration du branching
│   ├── 🖼️ merge-vs-rebase.png      --> Comparaison merge/rebase
│   └── 📂 svg                      --> Sous-dossier pour les icônes SVG
│       ├── 📄 branch-icon.svg
│       ├── 📄 commit-icon.svg
│       └── 📄 merge-icon.svg
```
---

<p align="center">
  <a href="GuideGit/demarrer-Git.md">Suivant</a>
</p>




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
