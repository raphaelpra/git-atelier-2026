# `git diff` en 10 lignes :

**À quoi ça sert** : Afficher les différences entre les versions de l'espace de travail et l'index, pour un ou tous les fichier du dépôt.

**La forme courante** : `git diff <fichier>`

**Un exemple qu'on peut taper** (testé dans `git-carnet`) :

```bash
git diff #on regarde tous les fichiers qui ont deux versions différentes, et leur différences
git diff README.md    # on regarde les differences entre les deux versions de README.md
```
**Ce que ça affiche / ce que ça change** : 
La sortie de `git diff` contient

    en - rouge les lignes supprimées

    en + vert les lignes ajoutées

    entre @@ et @@ des informations que l'on  peut ignorer (à destination d’outils graphiques, qui savent ainsi retrouver le contexte)

En revanche, git `diff` ne modifie rien.

**Le piège** ⚠️ : `git diff` affiche les différence entre l'espace de travail et l'index, pas celles entre l'index et le repository.

**Commande voisine** : `git diff --cached` - affiche les différences entre l'index et le repository.

Auteur : Anton Morisset (@zap174)