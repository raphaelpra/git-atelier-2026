# `git switch` en 10 lignes

**À quoi ça sert** : passer d'une branche à une autre

**La forme courante** : `git switch <autre branche>` (sans argument : `HEAD`, le dernier commit)

**Un exemple qu'on peut taper** (testé dans `git-carnet`) :

```bash
git switch main 

**Ce que ça affiche / ce que ça change** : on va vers la branche main

**Le piège** ⚠️ : ne créer pas ue nouvelle branche, elle doit déjà exister

**Commande voisine** : `git branch <nouvelle branche>` créer une nouvelle branche 

Auteur : Grégoire Saulquin (`@gregoiresaulquin12-cmyk`)
