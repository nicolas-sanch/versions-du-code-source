# 2 - Créer et manipuler un dépôt local

Pour créer un dépôt local:
```sh
mkdir mon-dossier
cd mon-dossier
git init # Initialise un nouveau dépôt dans le répertoire courant
code .   # Pour ouvrir notre IDE
```

Git créer par défaut une branche _master_ <br/>
Le contenu du dépôt est hébergé dans le dossier _.git_ généré<br/>

Nous pouvons visualiser son contenu avec la commande ```ls -la .git```

## Trois zones

Après l'initialisation de notre dépôt, nos fichiers évoluent entre trois zones :
* Le répertoire de travail qui correspond au dossier du projet stocké sur le disque dur,
* L'index où l'on trouve les fichiers en attente de commit,
* Le dépôt qui contient tous les commits (toute l'historique).

```git status``` permet de visualiser l'état des fichiers
<br/>

![Trois_zones.pgn](https://github.com/nicolas-sanch/versions-du-code-source/blob/main/2_Depot/Trois_zones.png)


## Ajouter des fichiers dans l'index

```sh
git add mon_fichier  # Pour ajouter le fichier "mon_fichier"
git add -A           # Pour ajouter tous les fichiers
```

## Ajouter des fichiers au dépôt

```sh
git commit -m "lorem ipsum"
```

Cette commande est l'élément central de Git. <br/>
Le [commit](https://git-scm.com/docs/git-commit/fr) _doit_ représenter un ensemble de modifications cohérentes entre elles.

## Visualiser les détails des commits

```sh
git log -1 # -1 Pour afficher le commit le plus récent
```

## Identifier l'auteur d'une ligne de code

```sh
git blame mon_fichier
```

---

⬅️ [1_Configuration](https://github.com/nicolas-sanch/versions-du-code-source/1_Configuration/blob/main/README.md) | [3_Branches](https://github.com/nicolas-sanch/versions-du-code-source/blob/main/3_Branches/README.md)  ➡️
