## Etapes à réaliser après avoir créer une Repo sur GitHub

Ouvrir git et se rendre sur le dossier dans lequel se trouve notre projet

- `git init`
- `git status`
- `git add .`
- `git commit -m "V1.0"`
- `git remote add origin 'url du repo'`
- `git fetch origin`
- `git merge origin/main --allow-unrelated-histories`
- `git status`
- `git add .`
- `git commit -m ""`
- `git push origin main`

### Etapes à réaliser pour cloner un projet sur GitHub

1. Cliquer et copier le lien HTTPS depuis "code"
   Ex : "https://github.com/Delgorithm/git-learning.git"

2. Utiliser iTerm pour se rendre dans le dossier où on souhaite placer le projet GitHub
   Ex : Downloads -> Projet -> E-commerce : Delgomania

3. Faire la commande :

   - `git clone "url"`

   Ex : `git clone https://github.com/Delgorithm/git-learning.git`

4. Rentrer dans le dossier pour vérifier si tout est bon. Puis sortir de celui-ci

5. Coder le projet :

   - code git-learning

## Tips and Tricks

### Combine "add" & "commit

A la place de faire :

- `git add .`
- `git commit -m "V1.0"`
  On peut directement fusionner les 2 commandes d'un trait :

Commande :

- `git commit -am "V1.0"`

### --amend

Permet de modifier le dernier commit que l'on souhaite modifier
Permet de :

- Changer le message du commit
- Ajouter/supprimer des fichiers du dernier commit
- Modifier les contenus du dernier commit

Commande :

- `git commit --amend` (Permettra de modifier le dernier message)

- `git commit --amend -a` (Permettra de modifier le contenu des fichiers du dernier commit)

#### Point importants :

- Nécessité de "`push`" avec la commande "git push --force" pour pouvoir appliquer les modifications obtenu via "`--amend`"
- Si on a déjà partagé la branche avec d'autres utilisateurs, il est recommandé de ne pas utiliser cette commande, car elle peut causer des problèmes de fusion lorsqu'ils essaient de récupérer votre dernière version de la branche.

## Pretty logs

Pour obtenir un graphique représentant nos différents commits qui ont eu lieu :

Commande :

- `git log --graph --online --decorate`

## Next tips to write about :

- `git rebase`
- `git init --bare`
- `--force-with-lease`
