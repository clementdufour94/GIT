git init
git branch dev : créer une branche
git branch : Afficher maintenant l’ensemble des branches se trouvant sur notre dépôt
git checkout dev : déplacer le HEAD sur la branche dev
git checkout master : déplacer le HEAD sur la branche master
git checkout -b feature_header : 
git branch -d : supprimer la branche
git branch -D : forcer la suppression d'une branche
git merge dev : merge dev dans master
git merge dev --no-ff : faire un commit de merge même si on estdans une situation sans divergence de branche
git branch --no-merged : Lister toutes les branches non mergées
git stash : remiser le code qui n'est pas fini
git stash list : Listez sur la branche les stash
git stash apply : Récuperer ce qui était dans la stash et l'appliquer => récupération de son code modifié
git stash drop : supprimer ce qui se trouve dans la remise
git stash apply stash : appliquer un stash particulier
git push : permet de publier une branche distante
git remote : Inspecter un dépôt distant