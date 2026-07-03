# Correction J1 partie I : les bases

1. Question (Q) : créez un nouveau dossier de travail
2. Q2 : initialisez un dépôt git
```bash
# Réponse (R)
# Au préalable, placez-vous dans votre dossier de travail depuis le terminal
git init
```
3. Q3 : effectuez la liaison entre votre dépôt local et le dépôt distant sur gitHub, GitLab ou BitBucket
```bash
# R3 en remplaçant https://github.com/glo10/11122025-git.git par l'URL de votre dépôt distant
git remote add origin https://github.com/glo10/11122025-git.git
```
4. Q4 : créez un fichier *.gitignore* excluant le dossier *img*.
- R4 : cf [.gitignore](./.gitignore)
```bash
# R4 contenu du fichier .gitignore
**/img # ** tous les niveaux des dossiers, parent, dossier, sous sous-dossier, etc.
```
5. Q5 : effectuez votre premier commit
```bash
# R5
git add .gitignore
git commit -m "first commit"
```
6. Q6 : renommez le nom de la branche *master* en *main* 
```bash
# R6
git branch -M main
```
7. Q7 : créez et (dé)placez-vous dans une branche nommée *feature/j1/p1*
```bash
# R7
git checkout -b feature/j1/p1
```
8. Q8 : créez un dossier *img*
- R8 : cf. [/img/](./img/)
9. Q9 : ajoutez le fichier *.gitkeep* dans *img*.
- R9 : cf. [/img/.gitkeep](./img/.gitkeep)
10. Q10 : effectuez un commit en respectant la convention de nommage Angular.
```bash
# R10
# Pour versionner le dossier /img/, 2 options soit enlever le dossier du .gitignore
# soit faire un git add -f img/
git add -f img/
git commit -m "refactor: add folder /img/"
```
11. Q11 : créez un fichier README.md à la racine contenant une liste des objets de votre choix parmi la liste suivante ou à partir de votre imagination débordante :
- Fruits
- Voitures
- Sandwich
- Jeux
- Films
- Etc.
```bash
# R11
```
- cf [README.md](README.md)
12. Q12 : effectuez un ou plusieurs commits sur cette branche *feature/j1/p1*
```bash
# R12
git add README.md
git commit -m "refactor: add README.md"
```