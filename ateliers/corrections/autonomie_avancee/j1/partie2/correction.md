# Correction J1 partie II : consolidation

1. Q1 : créez une nouvelle branche *feature/j1/p2*
```bash
# Réponse (R1)
git checkout main # création depuis la branche principale main
git checkout -b feature/j1/p2
```
2. Q2 : créez le fichier *README.md* avec une autre liste d'objet.
- R2 : cf [README.md](README.md)
3. Q3 : faites une capture d’écran de l’état de votre dépôt et enregistrez le fichier dans le dossier *img/*.
- R3 : cf dossier [img/](./img/)
4. Q4 : effectuez un commit votre travail en respectant les bonnes pratiques de commit [voir l'annexe partie commits](./../annexe.md).
```bash
# R4
git add README.md img/
git commit -m "feat: new fruits"
```
5. Q5 : faites une nouvelle capture d’écran de votre dépôt et enregistrez le fichier dans le dossier *img/*.
- R5 : cf. dossier [img/](./img/)
6. Q6 : retirez la ligne contenant *img* dans le *.gitignore*.
- R6 : cf. fichier [.gitignore](./.gitignore)
7. Q7 : effectuez un commit
```bash
# R7
git commit -am "refactor: remove img/ from .gitignore"
```