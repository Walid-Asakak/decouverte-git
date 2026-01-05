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

