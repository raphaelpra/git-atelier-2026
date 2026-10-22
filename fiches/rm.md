# `git rm` en 10 lignes

**À quoi ça sert** : supprimer un fichier à la fois du répertoire de travail et de l’index, pour que sa suppression soit prête à être commitée.

**La forme courante** : `git rm [options] fichier`

**Un exemple qu'on peut taper** : 

```bash
touch brouillon.txt
git rm brouillon.txt
git status
```

**Ce que ça affiche / ce que ça change** : git rm affiche rm 'brouillon.txt'. Le fichier disparaît du disque et git status le montre dans « Changes to be committed » comme deleted: brouillon.txt. Il ne reste plus qu’à faire un git commit.

**Le piège** ⚠️ : si le fichier a des modifications non commitées, Git refuse de le supprimer, et -f les écrase définitivement.

**Commande voisine** : `git rm --cached <fichier>` – retire le fichier de l’index (Git cesse de le suivre) mais le laisse sur le disque, alors que git rm seul le supprime aussi du disque.
Auteur : Prénom Nom (`@GeraudRoussel`)
