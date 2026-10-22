# `git cherry-pick` en 10 lignes

**À quoi ça sert** : appliquer sur la branche courante les modifications d’un ou plusieurs commits précis provenant d’une autre branche, sans intégrer toute cette branche.

**La forme courante** : `git cherry-pick <commit-hash>`

**Un exemple qu'on peut taper** (testé dans `git-carnet`) :

```bash
git cherry-pick commit-hash ...
```

**Ce que ça affiche / ce que ça change** : rajoute des commits à la branche principale.


Auteur : Esther Balu (`@EstherBalu`)
