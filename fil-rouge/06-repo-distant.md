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