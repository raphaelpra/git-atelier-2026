# `git rm` en 10 lignes

**À quoi ça sert** : supprimer des fichiers de l'espace de travail

**La forme courante** : `git rm rf <nom du fichier>`

**Un exemple qu'on peut taper** (testé dans `git-carnet`) :

```bash
rm git-atelier-2026  # à ne pas faire si on veut garder le dossier
```

**Ce que ça affiche / ce que ça change** : supprime le dossier git-atelier-2026 de la liste des fichiers du répertoire.

**Le piège** ⚠️ : Ne pas supprimer le .git sinon on a plus de git dans ce répertoire.

**Commande voisine** : `git rm --cached` – retire de l'index mais existe toujours

Auteur : Prénom Nom (`@gregoiresaulquin12-cmyk`)
