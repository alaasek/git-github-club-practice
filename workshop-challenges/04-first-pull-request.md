# Challenge 04 — Your First Pull Request | Défi 04 — Votre première Pull Request

**Level / Niveau:** Collaboration / Collaboration

## Goal | Objectif

**EN:** Contribute to the club repository using the fork-and-pull-request workflow.  
**FR :** Contribuer au dépôt du club en utilisant le workflow fork et Pull Request.

**This challenge is planned for the later practical test.**  
**Ce défi est prévu pour le test pratique ultérieur.**

## Steps | Étapes

1. Fork the club repository on GitHub. / Créez un fork du dépôt du club sur GitHub.
2. Clone your fork. / Clonez votre fork.
   ```bash
   git clone <your-fork-url>
   ```
3. Create a feature branch. / Créez une branche de fonctionnalité.
   ```bash
   git switch -c add-my-contribution
   ```
4. Make one small approved change. / Effectuez une petite modification autorisée.
5. Stage and commit it. / Préparez et enregistrez-la.
   ```bash
   git add <file>
   git commit -m "docs: add my contribution"
   ```
6. Push your branch to your fork. / Envoyez votre branche vers votre fork.
   ```bash
   git push -u origin add-my-contribution
   ```
7. Open a Pull Request from your branch to the club repository's `main` branch. / Ouvrez une Pull Request de votre branche vers `main` dans le dépôt du club.
8. Describe what changed and why. / Décrivez ce qui a changé et pourquoi.

## Good Pull Request habits | Bonnes pratiques

- Keep one PR focused on one task. / Limitez chaque PR à une seule tâche.
- Use a clear title and description. / Utilisez un titre et une description clairs.
- Be respectful during review. / Restez respectueux pendant la revue.
