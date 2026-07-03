# Correction atelier 3.1 : comprendre les principes de git

## Objectifs

- [x] Cloner des projets distants
- [x] Explorer l'historique d'un projet Git

## Compétences validées

- [x] Utiliser la commande `git clone` pour cloner un projet distant (depuis GitHub, GitLab, BitBucket)
- [x] Utiliser la commande `git log` pour voir l'historique des commandes


## Synthèse commandes

|                                            | Commande                                    |
| ------------------------------------------ | ------------------------------------------- |
| Cloner un dépôt distant à partir de son URL         | `git clone URL`                 |
| Lire l'historique        | `git log`                 |

## Correction

1. Q1 : clonez les dépôts contenant les frameworks JS
- [https://github.com/facebook/react](https://github.com/facebook/react)
- [https://github.com/angular/angular](https://github.com/angular/angular)
- [https://github.com/vuejs/core](https://github.com/vuejs/core)

```bash
# R1
git clone https://github.com/facebook/react
git clone https://github.com/angular/angular
git clone https://github.com/vuejs/core
```

2. Q2 : explorez l'historique à l'aide des commandes suivantes :
- Depuis un des 3 trois dépôts, exécutez les commandes suivantes
- `git log --oneline`
- `git log --graph --all`
```bash
# R2
git log --oneline
git log --graph --all
```

3. Q3 : explorez le Web et cloner un projet git de votre choix.
- R3 : vous avez l'embarras du choix depuis [GitHub](https://github.com) avec tous les dépôts