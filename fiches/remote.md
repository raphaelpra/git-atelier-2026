# `git remote` en 10 lignes

**À quoi ça sert** : gérer les noms et les adresses des dépôts distants associés au dépôt local.

**La forme courante** : `git remote add <nom> <URL>`

**Un exemple qu'on peut taper** :

```bash
git remote add upstream https://github.com/raphaelpra/git-atelier-2026.git
git remote -v
```

**Ce que ça affiche / ce que ça change** : enregistre le surnom `upstream`, puis affiche les noms et URL des remotes pour la récupération (`fetch`) et l'envoi (`push`), sans télécharger de commits ni modifier les fichiers du projet.

**Le piège** ⚠️ : une ligne `(push)` dans `git remote -v` ne garantit pas le droit d'écrire dans le dépôt distant.

**Commande voisine** : `git fetch` – récupère les nouveaux commits d'un dépôt distant, tandis que `git remote` gère les connexions configurées.

Auteur : Sean Bellamy (`@sean-bellamy`)