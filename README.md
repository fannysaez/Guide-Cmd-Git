<p align="center">
  <img src="./assets/svg/git-commands-logo.svg" width="500" alt="Logo">
</p>

---

# 30 commandes Git utiles à connaître pour mieux gérer ton code

Quand on commence à utiliser Git, on se limite souvent à git add, git commit, et git push...
Mais Git propose bien plus pour suivre, tester, corriger ou organiser son travail au quotidien.

Voici une sélection de 30 commandes que je trouve pratiques :

---

## 1. Démarrer avec Git

#### `git init`
→ Crée un dépôt Git vide dans le dossier actuel (pour commencer à versionner un projet).

#### `git clone [url]`
→ Récupère un projet depuis un dépôt en ligne (GitHub, GitLab...) et le copie sur votre machine.

#### `git config --global user.name "TonNom"`
→ Définit ton nom d'auteur pour tous les projets.

#### `git config --global user.email "email@example.com"`
→ Idem pour l'adresse email associée aux commits.

---

## 2. Suivre les changements

#### `git status`
→ Affiche les fichiers modifiés, ajoutés ou supprimés.

#### `git add [fichier]`
→ Prépare un fichier pour le commit (le place dans la "staging area").

#### `git add .`
→ Ajoute tous les fichiers modifiés à la staging area.

#### `git commit -m "Message"`
→ Enregistre officiellement les modifications avec un message descriptif.

#### `git commit --amend`
→ Modifie le dernier commit (pour corriger un oubli ou un message).

---

## 3. Travailler avec des branches

#### `git branch`
→ Affiche la liste des branches existantes.

#### `git branch nom_branche`
→ Crée une nouvelle branche.

#### `git checkout nom_branche`
→ Change de branche.

#### `git checkout -b nom_branche`
→ Crée une branche ET bascule dessus directement.

#### `git merge nom_branche`
→ Fusionne une branche dans celle en cours.

#### `git branch -d nom_branche`
→ Supprime une branche locale.

---

## 4. Travailler avec un dépôt distant (ex : GitHub)

#### `git remote -v`
→ Liste les dépôts distants (pour voir si ton projet est lié à GitHub).

#### `git remote add origin [url]`
→ Connecte ton dépôt local à un dépôt distant.

#### `git push origin branche`
→ Envoie ton code vers le dépôt distant.

#### `git pull origin branche`
→ Récupère et fusionne les modifs du dépôt distant.

#### `git fetch origin`
→ Récupère les modifs du dépôt sans les fusionner automatiquement.

---

## 5. Consulter l'historique et les changements

#### `git log`
→ Liste tous les commits effectués.

#### `git log --oneline`
→ Affiche les commits en version compacte.

#### `git diff`
→ Montre les différences non ajoutées (entre fichier modifié et version enregistrée).

#### `git diff --staged`
→ Montre les différences déjà ajoutées (en attente de commit).

---

## 6. Annuler, restaurer ou mettre de côté

#### `git reset fichier`
→ Enlève un fichier de la staging area (mais garde les modifs).

#### `git reset --hard [commit]`
→ Repart sur un ancien commit et supprime tout ce qu'il y a après.

#### `git stash`
→ Sauvegarde temporairement les modifs en cours (pour changer de branche sans perdre).

#### `git stash pop`
→ Récupère les modifications mises de côté.

---

## 7. Pour aller plus loin

#### `git rebase branche`
→ Rejoue les commits d'une branche sur une autre, pour un historique plus propre.

#### `git cherry-pick [commit]`
→ Applique un commit précis sur ta branche actuelle (sans tout fusionner).

---

*Astuce : Enregistre ce fichier comme mémo personnel ou partage-le avec ton équipe pour vous aider à mieux exploiter Git !*