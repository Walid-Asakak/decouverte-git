# Je veux partager mon code sur un dépôt distant :

- Prendre mon code et le mettre sur github
- Je dois me connecter sur Github (avec profil)
- Je dois créer un repository sur Github (le nom du projet)
- Je dois copier les commandes suivantes : 

'''sh
# Associer le repository local avec le repository distant :
git remote add origin adresse_projet

# On prend l'ensemble des commits enregistrés dans notre ordinateur (en local)
# et les envoyer (push) sur le repository distant :
git push -u origin main
'''



# Cas pratique : 

Dans le fichier index.html, ajouter à la fin du fichier dans la balise footer un formulaire avec 2 champs.
Un champ input de type email qui permet à l'utilisateur de s'inscrire à une newsletter et un button pour soumettre le formulaire.

Une fois que ce code est saisi, vous allez faire :
git add .
git commit -m"feat(home) formulaire newsletter"
git push

Enfin, regardez sur Github si le commit a bien été ajouté