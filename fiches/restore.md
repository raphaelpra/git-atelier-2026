# `git <commande>` en 10 lignes

**À quoi ça sert** : Annuler des modifications locales non validées (working directory), voire retourner au contenu de n'importe quel commit.

**La forme courante** : 
```bash
git restore <fichier>        # restaure les fichiers depuis l'index (zone de staging)
git restore .                # tous les fichiers modifiés du dossier courant
git restore --staged <fichier>   # retire le fichier de la zone de staging (sans toucher au contenu du fichier) — remplace « git reset HEAD fichier »
git restore --source=<commit> <fichier>   # restaure depuis un commit précis (ou une branche)
```
**Un exemple qu'on peut taper** (testé dans `git-carnet`) :

```bash
echo "test" >> README.md   # modifie un fichier
git status                 # → modified: README.md (rouge)
git restore README.md      # le fichier retrouve son dernier état indexé/validé
git status                 # → nothing to commit, working tree clean
```

**Ce que ça affiche / ce que ça change** : 
Rien à l'écran en cas de succès : la commande est silencieuse.


**Le piège** ⚠️ : git restore est destructif et sans filet : contrairement à un commit, un revert ou un stash, il n'y a aucune corbeille, aucune confirmation, aucun moyen de récupérer les modifications perdues.

**Commande voisine** : `git checkout` – checkout sert à la fois à basculer de branche et à restaurer des fichiers. C'est exactement cette ambigüité qui a motivé la scission : git switch (changer de branche) + git restore (restaurer des fichiers).

Auteur : Théophane Point--Mulon (`@TheophanePM`)
