git config --local user.name Tony : mettre nos noms
git config --local user.email tony@tony.fr : mettre nos mails
git--no-pager log --oneline : consulter l'historique sans pagination
git--no-pager log -3 --oneline : pour 3 commits
git log --oneline -2 : consulter les 2 derniers commits
git log --author "Antoine07" : consuter le commit de l'utilisateur
git log --since=1.day
git log --before="2019-09-01"
git log calzone.txt : consulter l'historique d'un fichier
git log -p
git log -2 -p
git log -p calzone.txt : visualiser les modifications au sein d'un fichier ou de l'ensemble/d'un ensemble des fichier(s)
git log --stat calzone.txt : visualiser les statistiques desmodifications des fichiers
git log -E -i --grep='Pizza' : rechercher des logs (messages des commits) :E expression pour rechercher les/l’occurence(s) et i pour insensible à la casse(majuscule/minuscule)
git blame calzone.txt : corrige la/les modification(s) dans l’application
git diff : avant d'indexer un fichier, visualiser les modifications
git diff --cached : affiche les différences entre le dernier commit et l’index
git diff HEAD~1 : pour reculé d’un commit en arrière.
git diff HEAD~3 HEAD :  visualiser les différences entre le HEAD et un état antérieur dudépôt, par exemple 3 commits avant
git log --oneline : Récupérez les haches des deux derniers commits
git log f5541d6 b058c4f : les logs entre deux commits
git diff --stat : faire des stats sur les différences opérées dans les fichiers
git restore calzone.txt : remettre le dépôt dans l’état dans lequel il se trouvait juste avant une modification
git restore --staged :  refaire la modification et ajouter le fichier dans l’index
git reset HEAD~1 : Annule le dernier commit et met tout dans le WD sans perte
git reset --soft HEAD~1 : Annule le dernier commit et met tout dans la staging area sans perte
124f561 (HEAD -> master) file33 
6695308 file22
0637561 file11
8ef0ef2 ignore
0a70edb file2
bf3f73c first commit 
git reset 8ef0ef2 : Le HEAD -> master se déplacera sur le commit 8ef0ef2 en annulant les autres commits sans perte
git reset –hard : Annule le dernier commit et supprime les modifications...(danger)
git checkout : remettre un fichier dans son état initial
git revert 419e298 :  créer un commit revert d’annulation du dernier commit réalisé