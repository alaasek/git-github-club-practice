# Common Git Errors | Erreurs Git fréquentes

Use this guide to understand the message before choosing a command.
Utilisez ce guide pour comprendre le message avant de choisir une commande.

## 1. `fatal: not a git repository`

**EN:** Your terminal is not inside a Git repository.  
**FR :** Votre terminal ne se trouve pas dans un dépôt Git.

**Try | À essayer:**
```bash
pwd
ls
cd <project-folder>
git status
```

## 2. `Author identity unknown`

**EN:** Git does not know which name and email to attach to your commits.  
**FR :** Git ne connaît pas le nom et l'adresse e-mail à associer à vos commits.

```bash
git config --global user.name "Your Name"
git config --global user.email "you@example.com"
```

Use an email you are comfortable associating with your commits.
Utilisez une adresse e-mail que vous acceptez d'associer à vos commits.

## 3. `nothing to commit, working tree clean`

**EN:** Git sees no new changes to commit. This is usually a normal status, not an error.  
**FR :** Git ne détecte aucune nouvelle modification à enregistrer. C'est généralement un état normal, pas une erreur.

```bash
git status
```

## 4. `rejected (non-fast-forward)`

**EN:** The remote branch has commits that your local branch does not contain. Fetch and inspect before integrating.  
**FR :** La branche distante contient des commits absents de votre branche locale. Récupérez et examinez l'historique avant de l'intégrer.

```bash
git fetch origin
git log --oneline --graph --decorate --all -15
```

Then decide whether a merge or rebase is appropriate. If unsure, ask for help before using force push.
Ensuite, déterminez si un merge ou un rebase convient. En cas de doute, demandez de l'aide avant d'utiliser `force push`.

## 5. `You have not concluded your merge (MERGE_HEAD exists)`

**EN:** A merge is already in progress. Check its state before starting another merge or pull.  
**FR :** Un merge est déjà en cours. Vérifiez son état avant de lancer un autre merge ou pull.

```bash
git status
```

Follow Git's instructions. If conflicts are listed, resolve them carefully, stage the resolved files, and complete the merge commit.
Suivez les indications de Git. Si des conflits sont listés, résolvez-les soigneusement, ajoutez les fichiers résolus à la zone de préparation, puis terminez le merge avec un commit.

## 6. Merge conflict | Conflit de fusion

**EN:** Git cannot automatically combine overlapping edits. Open each conflicted file, choose the intended final content, remove conflict markers, then stage the resolved file.  
**FR :** Git ne peut pas combiner automatiquement des modifications qui se chevauchent. Ouvrez chaque fichier en conflit, choisissez le contenu final souhaité, supprimez les marqueurs de conflit, puis ajoutez le fichier résolu à la zone de préparation.

```bash
git status
git add <resolved-file>
git commit
```

## Safety reminder | Rappel de sécurité

**EN:** Do not copy commands such as `git reset --hard` or `git push --force` from a random tutorial. They can discard work or overwrite remote history. Understand the situation first.  
**FR :** Ne copiez pas des commandes comme `git reset --hard` ou `git push --force` depuis un tutoriel quelconque. Elles peuvent supprimer du travail ou écraser l'historique distant. Comprenez d'abord la situation.
