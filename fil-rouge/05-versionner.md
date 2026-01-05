# Les commandes de versionning 

-créer / modifier / supprimer un fichier
-Ctrl + s 


'''sh
git add .
git commit -m"texte explicatif sur le commit réalisé"


# Visualiser les commits : 
- 'gitk'
'''

# Comprendre la commande git add :
- Etape AVANT la création du COMMIT (enregistrement de la version)
- permet de lister l'ensemble des fichiers que l'on veut COMMIT
- Pour que le commit soit associé clairement aux fichiers concernés par la version

Quand un fichier est modifié ET que l'on vient de faire un git add =>
On dit que le fichier est dans un état 'staged' (en attente de versionning)

# Connaitre l'état de chaque fichier : 

'''sh
git status 
'''


Untracked files : fil-rouge/05-versionner.md

'''sh
(C'est la même commande)
git add .  
git add -A
git add --all 
'''

'''sh
git status 

git commit -m"ajout d'un footer"
'''

'''sh
git status 

nothing to commit, working tree clean => 
'''

# Il est possible de fusionner les deux commandes git add et git commit

/!!\ Attention cette commande ne fonctionne QUE pour les fichiers qui ont déjà été au moins une fois add :

'''sh
git commit -a -m "modification ..." 
'''

# Visualiser les commits :

- gitk
- git log (Appuyer sur la touche Enter => passer à la suite & appuyer sur la touche q pour sortir)
- git log --oneline

Quand on fait git log --oneline : 
'''txt
06da6d7 (HEAD -> main) toggle btn home (où je suis en train de regarder actuellement)
6a763bd modification ...
8696540 ajout d'un footer
4615dd0 ajouter des classes pour le  bouton
d47845c bouton toggle
abfbc37 ajout d'une barre de menu
9b26718 ajout de boostrap css
c12861a (origin/main) config git # sur github la version disponible est celle-ci
'''

Cas pratique : Pouvez-vous revenir dans le passé :

'''sh
git status
git add .
git commit -m"validation"
git log --oneline
git checkout hash => aller dans le passé
git checkout main => revenir dans le présent
'''

# Normer les descriptions dans les commits

/!\ Ce n'est pas obligatoire
MAIS ça permet de mieux s'y retrouver dans les commits => respecter la règle suivante : 

git add . 
git commit -m"type(portée description)" 
-le type => le type de code que je suis en train de réaliser 
            - fix => correctif
            - feat => fonctionnalité (ajouter une nouvelle fonctionnalité)
            - hotfix => correctif critique (en production)
            - docs => documentation / explication 
            - refactor => réorganisation du code

La portée : Quelle est la portée du commit => global / page index.html etc...

description : git add .
              git commit -m"docs(global) comment nommer les commits"