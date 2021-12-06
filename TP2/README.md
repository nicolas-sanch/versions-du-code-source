# Git distribué

## Prérequis

* Chaque élève doit avoir un compte github.<br/>
* Créer des groupes de 3-4 élèves et désigner un admin-git

## I - Mise en place

* admin-git créé un dépôt local
* il ajoute un fichier README.md avec le contenu suivant et commit
```txt
01 Nom:
01 Prénom:
02 Nom:
02 Prénom:
03 Nom:
03 Prénom:
04 Nom:
04 Prénom:
```
* il créé sur github un dépôt vide
* il pousse son dépôt local sur github

## II - Avec les droits en écriture

* admin-git invite les autres memebres du groupe (ils doivent communiquer leur id github)
* il donne les droits en écriture sur le dépôt au membres
* les membres clônent le dépôt en local
* chacun change le nom et prénom au numéro choisi
* tout le monde pousse

## III - Sans les droits en écriture

* admin-git créé un nouveau dépôt github vide
* il pousse son dépôt local sur github
Les membres doivent passer par l'étape _fork_ et _pull request_ pour transmettre leur contribution.<br/>
Une des façon de faire est la suivante :
* les membres commencent par cloner le dépôt de admin-git
* ils modifient le fichier local et commit
* ils retournent sur github pour créer un fork
* ils déclarent un nouveau remote```git remote add mine https://xxxxxxxx```
* les membres peuvent pousser sur leur fork et créer un pull request pour demander au leader d'intégrer leur contribution
<br/>
* La suppression d'un dépôt github se fait en allant tout en bas de la page _settings_
