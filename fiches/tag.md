# `git <commande>` en 10 lignes

**À quoi ça sert** : La commande git tag permet de créer des points de repère immuables dans l'historique de votre projet, le plus souvent pour marquer des numéros de version spécifiques.

**La forme courante** : `git tag [options] <argument>`

**Un exemple qu'on peut taper** (testé dans `git-carnet`) : git tag -a v1.0.0 -m "Release de la version 1.0.0"

```bash
git <commande> ...
```

**Ce que ça affiche / ce que ça change** : Un tag Git affiche un repère visuel fixe sur un commit spécifique dans l'historique et ne change absolument rien au code ou aux fichiers de votre projet

**Le piège** ⚠️ : • Le piège principal est d'oublier que les tags ne sont pas envoyés automatiquement sur le serveur distant lors d'un simple git push ; il faut explicitement utiliser git push origin --tags.

**Commande voisine** : •  La commande voisine est git branch, qui crée un pointeur mobile vers un commit (pour continuer à développer), contrairement au tag qui reste fixe dans le temps.


Auteur : Gwevenn Harrache (`@gwevenn`)
