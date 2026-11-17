# Git & GitHub Cheat Sheet | Fiche mémo Git & GitHub

A quick reference for the Data Science Club workshop at USTHB.
Une fiche de référence rapide pour l'atelier du Data Science Club à l'USTHB.

## 1. Setup | Configuration

```bash
git --version
git config --global user.name "Your Name"
git config --global user.email "you@example.com"
git config --global --list
```

**EN:** Check your Git installation and configure the name and email attached to your commits.  
**FR :** Vérifiez l'installation de Git et configurez le nom et l'adresse e-mail associés à vos commits.

## 2. Start a repository | Initialiser un dépôt

```bash
git init
git clone <repository-url>
git status
```

**EN:** `git init` creates a local repository. `git clone` copies an existing remote repository. `git status` shows the state of your working tree.  
**FR :** `git init` crée un dépôt local. `git clone` copie un dépôt distant existant. `git status` affiche l'état de votre espace de travail.

## 3. Stage and commit | Préparer et enregistrer

```bash
git add <file>
git add .
git diff
git diff --staged
git commit -m "docs: add workshop notes"
git log --oneline
```

**EN:** Stage the changes you want to include, inspect them, then save a snapshot with a commit.  
**FR :** Ajoutez les modifications à préparer, vérifiez-les, puis enregistrez un instantané avec un commit.

## 4. Branches | Branches

```bash
git branch
git switch -c feature/my-task
git switch main
git merge feature/my-task
git branch -d feature/my-task
```

**EN:** A branch lets you work on a change separately from the main line of development.  
**FR :** Une branche permet de travailler sur une modification séparément de la branche principale.

## 5. Connect to GitHub | Se connecter à GitHub

```bash
git remote -v
git remote add origin <repository-url>
git fetch origin
git pull origin main
git push -u origin main
```

**EN:** `fetch` downloads remote updates without integrating them. `pull` fetches and integrates. `push` uploads your commits.  
**FR :** `fetch` récupère les informations distantes sans les intégrer. `pull` récupère puis intègre les changements. `push` envoie vos commits.

## 6. Undo carefully | Annuler avec précaution

```bash
git restore <file>
git restore --staged <file>
git revert <commit-id>
```

**EN:** These commands have different effects. `restore` discards or unstages changes; `revert` creates a new commit that reverses an earlier commit. Check before using destructive commands.  
**FR :** Ces commandes ont des effets différents. `restore` annule des modifications ou retire un fichier de la zone de préparation ; `revert` crée un nouveau commit qui inverse un ancien commit. Vérifiez toujours avant d'utiliser une commande destructive.

## 7. Useful habits | Bonnes habitudes

- **EN:** Run `git status` often. **FR :** Exécutez souvent `git status`.
- **EN:** Make small, focused commits. **FR :** Faites des commits courts et ciblés.
- **EN:** Write meaningful commit messages. **FR :** Rédigez des messages de commit explicites.
- **EN:** Create a branch for each task. **FR :** Créez une branche pour chaque tâche.
- **EN:** Read the output before running the next command. **FR :** Lisez le résultat avant d'exécuter la commande suivante.
