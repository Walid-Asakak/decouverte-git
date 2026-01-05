# Les mots clés de git et github

# REPOSITORY (dépôt)
-ressemble à une base de données
-Le versionning réalisé par git va être stocké dans un dossier SPECIAL appelé " REPOSITORY " (C'est un dossier technique qui contient les différentes versions de notre code. On peut aussi appelé ça " REPO " ou "dépôt").

- Dépôt LOCAL (celui qui est enregistré dans notre ordinateur)
- Dépôt DISTANT (celui qui va être enregistré sur Github)

# COMMIT 
- COMMIT : Une version INCREMENTABLE de notre projet (incrémentable = version qui va stocker UNIQUEMENT les nouveautés)
-'git commit' Chaque commit a un nom qu'on lui donne ET une clé primaire (comme les bases de données) dite "hash"
- 1 COMMIT PAR FONCTIONNALITE
- HASH -> fonction qui permet de transformer un texte en chaîne de caractères (appelé hash OU empreinte)
- MD5() -> fonction de hashage
- google => MD5 générator => https://www.md5hashgenerator.com/s

Exemples de hash :
bonjour => Devient : 90403d695a7d41981925fbfc3be2b66b 
a => Devient : 0cc175b9c0f1b6a831c399e269772661

# FAIRE COMMUNIQUER REPO LOCAL AVEC REPO DISTANT 

-commande pour ENVOYER du code du LOCAL vers le DISTANT : 'git push'
-commande pour RECUPERER du code du DISTANT vers le LOCAL : 'git pull'
-1x par jour généralement (fin de journée / début de journée)

# Branch : 
-Créer des mondes parallèles 
-On a une nouvelle fonctionnalité que l'on souhaite créer MAIS on ne veut pas que ce code IMPACTE le travail DEJA EXISTANT.
-Git permet de créer un BRANCH => monde parallèle à notre projet (INDEPENDANT, QUI N'IMPACTE PAS LE PROJET EXISTANT)
-Par défaut on VERSIONNE sur la branch PRINCIPALE du projet qui s'appelle la branch 'main'