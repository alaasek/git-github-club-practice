# Git & GitHub Club Practice

Welcome to the **Data Science Club · USTHB** Git & GitHub practice repository!

This repository is a safe place to practise the workflow from your first commit to your first Pull Request.

## Learning Resources

New to Git or GitHub? Start with these resources:

- [Git Cheat Sheet](docs/GIT_CHEAT_SHEET.md) — Essential commands in English and French.
- [Git Glossary](docs/GLOSSARY.md) — Understand the key Git and GitHub terms.
- [Common Errors](docs/COMMON_ERRORS.md) — Troubleshoot frequent problems.

##  Workshop Goals

By completing the challenges, you will learn how to:

- Fork and clone a repository.
- Create a feature branch.
- Edit and stage a file.
- Make a meaningful commit.
- Push your branch to GitHub.
- Open a Pull Request for review.

##  Practice Challenges

Follow the guided exercises in the [`workshop-challenges/`](workshop-challenges/README.md) folder:

1. [Your First Commit](workshop-challenges/01-first-commit.md)
2. [Working with Branches](workshop-challenges/02-branches.md)
3. [Resolving Merge Conflicts](workshop-challenges/03-merge-conflicts.md)
4. [Your First Pull Request](workshop-challenges/04-first-pull-request.md)

##  Your First Contribution

1. If you are contributing to the club's original repository and do not have write access, click **Fork** on GitHub.
2. Clone your fork:

   ```bash
   git clone <your-fork-url>
   cd git-github-club-practice
   ```

3. Create a branch using your name or GitHub username:

   ```bash
   git switch -c docs/add-your-name
   ```

4. Open `CONTRIBUTORS.md` and add your name using the format already shown there.
5. Review your change:

   ```bash
   git status
   git diff
   ```

6. Stage and commit:

   ```bash
   git add CONTRIBUTORS.md
   git diff --staged
   git commit -m "docs: add <your-name> to contributors"
   ```

7. Push your branch:

   ```bash
   git push -u origin docs/add-your-name
   ```

8. On GitHub, open a Pull Request from your fork's branch to the original repository's `main` branch.
9. In the PR description, explain what you changed.

##  Contribution Rules

- Make one small, focused contribution per Pull Request.
- Use a descriptive branch name.
- Use a clear commit message.
- Do not commit passwords, API keys, tokens, `.env` files, virtual environments, or private data.
- Be respectful in reviews and discussions.
- Do not edit another contributor's entry without permission.

##  Suggested Branch Names

- `docs/add-your-name`
- `docs/improve-readme`
- `fix/fix-typo`
- `feature/add-resource`

##  Need Help?

Open an Issue in this repository and describe:

- What you were trying to do.
- The command you ran.
- The complete error message (remove any passwords, tokens, or private information).

Happy learning!