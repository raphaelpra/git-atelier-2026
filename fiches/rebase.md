# `git rebase` en 10 lignes

**À quoi ça sert** : Copier un les commits d'une branche sous une autre, perd l'historique des commits contrairement à merge mais l'évolution des commits est linéaire.

**La forme courante** : `git rebase 'branche'`

**Un exemple qu'on peut taper** (testé dans `git-carnet`) :

```bash
git rebase cuisson
```

**Ce que ça affiche / ce que ça change** : une ou deux lignes.

**Le piège** ⚠️ : rebase efface l'historique des commits, on perds leur ordre de création.

**Commande voisine** : `git merge` – permet également de fusionner deux branches, mais conserve l'historique. L'arbre es commits est cependant moins clair lorsque de nombreuses fusions sont réalisées.

Auteur : Rémi Fournier (`@FournierR-github`)
