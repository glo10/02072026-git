# Correction J1 partie V : dépôt distant

Depuis votre compte GitHub, à partir du dépôt où vous avez envoyé précédemment votre travail.
1. Q1: créez une nouvelle branche *feature/j1/p5* à partir de la branche *main* depuis GitHub.
- Réponse (R) cf. [vidéo création d'une nouvelle branche depuis GitHub](../../../videos/create_branch.mp4)
2. Q2 : modifiez le fichier *README.md* en ajoutant encore d'autres objets depuis GitHub et effectuez votre commit.
- R2 cf. [vidéo ajout nouveau contenu dans le README.md](../../../videos/update_from_github.mp4)
3. Q3 : à partir d'ici, toutes les opérations se font en local, récupérez les modifications du dépôt distant (aide commande à effectuer `git checkout -b feature/j1/p5 --track origin/feature/j1/p5`).
```bash
# R3
# depuis la branche main sinon faites git checkout main
git checkout -b feature/j1/p5 --track origin/feature/j1/p5
```
4. Q4 : fusionnez la branche *feature/j1/p5* dans la branche *main* en local.
```bash
# R4
git checkout main
git merge feature/j1/p5
```