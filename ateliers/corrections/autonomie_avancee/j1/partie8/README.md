# Correction J1 partie VIII : patch

1. Q1 : depuis la documentation de la commande `git format-patch`, créez un patch de plusieurs commit incluant le commit ayant ajouté le fameux objet dans le projet. L'extraction de votre patch doit se faire dans le dossier */patches* à la racine de votre projet.
```bash
# R1
# Remplacez ID_COMMIT_AVANT_COMMIT_FAMEUX_OBJET par l'identifiant du commit juste avant celui ayant introduit le sandwich végan
git format-patch -o ./patches ID_COMMIT_AVANT_COMMIT_FAMEUX_OBJET
```
2. Q2 : créez un nouveau projet Git, en dehors du projet en cours.
```bash
# R2
# Se placer en dehors du repertoire courant avec la commande cd puis effectuez la commande suivante
git init
```
3. Q3 : effectuez un premier commit sur ce nouveau dépôt.
```bash
# R3 : ajout d'un fichier README.md à la racine vide puis la commande suivante
git add README.md
git commit -m "first commit"
```
4. Q4 : copiez/collez le dossier patches/ d'un dépôt (celui d'extraction) à l'autre (vers le nouveau, celui qui va l'appliquer)
- R4 : réalisez le copier/coller comme indiqué dans la question précédente
5. Q5 : appliquez uniquement le patch ayant introduit le fameux objet et ignorez les autres fichiers du dossier /patches
```bash
# R5
git apply --3way ./patches/fichier_patch_associe_commit_introduction_fameux_objet.patch
```
PS : *fichier_patch_associe_commit_introduction_fameux_objet.patch* à remplacer par le nom du fichier ayant introduit le fameux objet dans le projet, fichier commençant par ***00*** et avec l'extension ***.patch***