# Challenge 03 — Understand Merge Conflicts | Défi 03 — Comprendre les conflits de fusion

**Level / Niveau:** Intermediate / Intermédiaire

## Goal | Objectif

**EN:** Understand why a merge conflict happens and how to resolve it in a controlled practice repository.  
**FR :** Comprendre pourquoi un conflit de fusion apparaît et comment le résoudre dans un dépôt d'exercice contrôlé.

## Preparation | Préparation

Use a disposable practice repository or ask the instructor to prepare two branches that edit the same line differently.
Utilisez un dépôt d'exercice jetable ou demandez à l'encadrant de préparer deux branches qui modifient différemment la même ligne.

## Steps | Étapes

1. Inspect the conflict message and run `git status`. / Lisez le message de conflit et exécutez `git status`.
2. Open the conflicted file. / Ouvrez le fichier en conflit.
3. Identify the conflict markers: `<<<<<<<`, `=======`, and `>>>>>>>`. / Repérez les marqueurs de conflit.
4. Decide what the final content should be, edit the file, and remove the markers. / Décidez du contenu final, modifiez le fichier et supprimez les marqueurs.
5. Stage the resolved file and complete the merge as Git instructs. / Ajoutez le fichier résolu et terminez le merge selon les indications de Git.

```bash
git status
git add <resolved-file>
git commit
```

**Safety / Sécurité:** Do this only in a practice repository. Never resolve a real project conflict by blindly choosing “ours” or “theirs”.
Faites cet exercice uniquement dans un dépôt de pratique. Ne résolvez jamais un conflit réel en choisissant aveuglément « ours » ou « theirs ».
