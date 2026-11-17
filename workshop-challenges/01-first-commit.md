# Challenge 01 — Your First Commit | Défi 01 — Votre premier commit

**Level / Niveau:** Beginner / Débutant

## Goal | Objectif

**EN:** Create a small file, stage it, and save your first commit.  
**FR :** Créer un petit fichier, le préparer, puis enregistrer votre premier commit.

## Steps | Étapes

1. Open your project folder in the terminal. / Ouvrez le dossier du projet dans le terminal.
2. Check the repository status. / Vérifiez l'état du dépôt.
   ```bash
   git status
   ```
3. Create a file named `hello-git.txt` and write one sentence in it. / Créez `hello-git.txt` et écrivez-y une phrase.
4. Stage the file. / Ajoutez le fichier à la zone de préparation.
   ```bash
   git add hello-git.txt
   ```
5. Review what is staged. / Vérifiez ce qui est préparé.
   ```bash
   git diff --staged
   ```
6. Commit the change. / Enregistrez la modification.
   ```bash
   git commit -m "docs: add hello git file"
   ```
7. Check the latest commit and status. / Vérifiez le dernier commit et l'état du dépôt.
   ```bash
   git log --oneline -1
   git status
   ```

## Reflection | Réflexion

- **EN:** What is the difference between `git add` and `git commit`?
- **FR :** Quelle est la différence entre `git add` et `git commit` ?
