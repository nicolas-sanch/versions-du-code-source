# TP

## Utilisation de Git stash

```git stash```va garder toutes les modifications de côté. Elles ne seront plus présentes dans le répertoire de travail et l'index, elles ne seront pas non plus présentes dans l'historique

### Exemple

```sh
mkdir git_stash
cd git_stash
git init
vi README
vi projet.md
git add -A
git commit -m "README + projet.md : ajout"
```

Après ce commit, nous poursuivons les modifications

```sh
vi projet.md  # On le modifie
vi index.html
git status
```

Nous mettons de côté les modifications effectuées

```sh
git stash --include-untracked
```

Puis nous récupérons les modification

```sh
git stash list            # Lister
git stash apply stash@{0} # Récupérer les modifications
git stash drop stash@{0}  # Supprimer le stash
```

## Création d'un dépôt distant pour un projet existant

```sh
mkdir local
cd local
git init
vi fichier.txt
git add fichier.txt
git commit
cd ..
mkdir serveur
cd serveur
git clone --bare ../local/.git clone_distant
cd clone_distant
git log
```