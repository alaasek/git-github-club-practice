# Challenge 02 — Work with Branches | Défi 02 — Travailler avec les branches

**Level / Niveau:** Beginner–Intermediate / Débutant–Intermédiaire

## Goal | Objectif

**EN:** Make a change on a separate branch and merge it into `main`.  
**FR :** Effectuer une modification sur une branche séparée puis l'intégrer dans `main`.

## Steps | Étapes

1. Check your current branch. / Vérifiez votre branche actuelle.
   ```bash
   git branch
   ```
2. Create and switch to a branch. / Créez une branche et basculez dessus.
   ```bash
   git switch -c docs/add-learning-goal
   ```
3. Add a short learning goal to a practice text file. / Ajoutez un court objectif d'apprentissage à un fichier de pratique.
4. Stage and commit your change. / Préparez et enregistrez votre modification.
   ```bash
   git add <file>
   git commit -m "docs: add learning goal"
   ```
5. Switch back to `main`. / Revenez sur `main`.
   ```bash
   git switch main
   ```
6. Merge your branch. / Intégrez votre branche.
   ```bash
   git merge docs/add-learning-goal
   ```
7. Review the history. / Examinez l'historique.
   ```bash
   git log --oneline --graph --decorate -10
   ```

## Reflection | Réflexion

- **EN:** Why is it useful to work on a branch instead of changing `main` directly?
- **FR :** Pourquoi est-il utile de travailler sur une branche plutôt que de modifier directement `main` ?
