# Dépôts distants

Le dépôt distant sert à centraliser un dépôt.<br/>
Il ne contient pas de répertoire de travail.

## Créer un dépôt distant

Un nouveau dépôt distant vierge se créer avec la commande : 
```sh
git init --bare mon_depot
```

Pour un projet existant localement, nous allons utiliser __depuis le serveur__ la commande :
```sh
git clone --bare path/to/local mon_depot
```

## Cloner un dépôt distant

Cloner un dépôt revient à copier tout le contenu du dépôt (Branches, commits etc...)<br/>
Cette action peut être réaliser via les 4 protocoles suivants :
* Local
* SSH
* HTTP(S)
* Git

Lors de l'utilisation de la commande ```git clone```, un dépôt distant (remote) nommé _origin_ est automatiquement renseigné dans le fichier _.git/config_<br/>
Il s'agit d'un raccourci vers le dépôt distant.

## Envoyer et recevoir ses modifications

```sh
git push origin master # Ici, nous précisons l'envoi au remote nommé origin les modifications ajoutées dans la branche master
```

```sh
git pull
```
Il s'agit d'un raccourci pour les commandes :
```sh
git fetch            # Télécharge les commits
git merge FETCH_HEAD # Intègre les modifications dans la branche locale
```

## Lister les dépôts distants liés au dépôt local

```sh
git remote
```

---

⬅️ [3_Branches](https://github.com/nicolas-sanch/versions-du-code-source/blob/main/3_Branches/README.md) | [TP1](https://github.com/nicolas-sanch/versions-du-code-source/blob/main/TP1/README.md)  ➡️