
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

---

</div>
<p align="center">
  <a href="Cmd-Git/demarrer-Git.md">Suivant</a>
</p>
