# `git <commande>` en 10 lignes

**À quoi ça sert** : envoyer les commits locaux vers un dépôt distant (comme GitHub, GitLab, etc.)

**La forme courante** : 'git push <dépôt> <branche>' (souvent réduit à git push si la branche est déjà liée au dépôt distant)

**Un exemple qu'on peut taper** (testé dans `git-carnet`) :

```bash
git push origin main        # envoie les commits de la branche courante vers origin/main
git push -u origin feature  # envoie la branche et mémorise le lien pour les futurs push
git push origin --tags      # envoie tous les tags locaux vers le dépôt distant
```

**Ce que ça affiche / ce que ça change** : l'état de l'envoi des données et des objets vers le serveur distant. Cela met à jour la branche correspondante sur le dépôt distant (avec git-carnet: Permission to raphaelpra/git-carnet.git denied to Growth-K, j'ai pas les permissions)

**Le piège** ⚠️ : Si le dépôt distant contient des commits que vous n'avez pas en local (par exemple modifiés par un collègue), le push est refusé. Il faut d'abord récupérer les modifications avec git pull.

**Commande voisine** : 'git pull' – pour récupérer et fusionner les modifications du dépôt distant vers le dépôt local.

Auteur : Kilian Taillandier (`@Growth-K`)
