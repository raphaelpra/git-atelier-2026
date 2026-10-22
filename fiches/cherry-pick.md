# `git <commande>` en 10 lignes

**À quoi ça sert** : copie et colle certains commits à la suite de la branche courante (ou d'un commit HEAD si détaché), permet de ne pas fusionner toute la branche. Il déplace le pointeur de la branche actuelle sur le dernier commit collé.

**La forme courante** : `git cherry-pick C1 C5 C8`

**Un exemple qu'on peut taper** (testé dans `git-carnet`) :

```bash
git cherry-pick z3rk5 ft9a3 cj8ie ...
```

**Ce que ça affiche / ce que ça change** : copie les commits (ici 3 distincts) dont les hash sont précisés dans la commande et les mets à la suite du HEAD actuel

**Le piège** ⚠️ : ça ne déplace pas les commits choisis, ça les copie/colle

**Commande voisine** : `git rebase -i` – cette dernière permet aussi de choisir certains commits dans une branche, mais elle les déplace avec la branche actuelle pour la mettre au bout d'une autre

Auteur : Tom Vicq (`@tomvicq-github`)
