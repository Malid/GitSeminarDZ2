# commandes GIT
1. **git config --global user.name "Name"** - définissez ou modifiez le nom d'utilisateur à afficher dans git.
2. **git config --global user.email "myemail@mail.com"** définir ou modifier l'adresse e-mail enregistrée dans git
3. **git init** - initialisation du dépôt
4. **git status** - vérifie l'état du dépôt
5. **git add filname.ext** ou **git add .** - ajouter des fichiers individuels ou tous les fichiers à la zone de staging
6. **git commit -m "Message About Commit"** - crée un commit
7. **git log** - afficher l'historique des commits avec les modifications
8. **git diff** - afficher les modifications avant de valider
9. **git checkout _<BranchName ou les premiers caractères du hash de commit>_** - saute à la branche ou au commit spécifié
10. **git checkout -b new_branch_name** - crée une nouvelle branche et bascule vers celle-ci
11. **git branch new_branch_name** - crée une nouvelle branche
13. **git branch** - voir la liste des branches
14. **git branch -d branch_to_delete** - supprimer une branche sans rien casser
15. **git merge branch_name** - Fusion de la branche spécifiée avec la branche actuelle
16. **git log --graph** - Afficher le journal de branche sous forme de graphique

*si vous créez un fichier **.gitignore** dans le référentiel et y ajoutez une liste de fichiers, tels que des images ou des fichiers volumineux, lorsque vous ajoutez le fichier **.gitignore** au référentiel, git ne les traitera pas des dossiers

**git log -n** Afficher les n derniers commits

**git log --since 2022-01-17 _until 2022-01-22_** affiche les commits à partir d'une date précise *jusqu'à une date précise (optionnel)*

**git rm _FileName_** supprime le fichier des index git

**git rebase main** copie un ensemble de commits et les déplace vers un autre emplacement

**git détacher HEAD** détacher HEAD de la branche pour valider

**git checkout main^** changer d'un niveau

**git checkout main~3** déplacer 3 commits en arrière

**git branch -f main HEAD~3** force la branche principale 3 parents à revenir de HEAD


***
# Pousser le dépôt local vers le serveur GitHub

**git remote add origin <_WebPatch.git_>**

**branche git -M principale**

**git push -u origin main**

**git push** pousse les modifications vers GitHub (_REQUIRES AUTHORIZATION_)

**git pull** téléchargement depuis le serveur. Tente de fusionner

**?git fetch** synchronise la branche locale avec la télécommande. Git pull appelle git fetch suivi de git merge
***
# Requête d'extraction Git

- Faire un **fork** (branche) du dépôt
- Faites un clone git de **notre** version du dépôt
- Créer une nouvelle branche et ** elle ** apporte nos modifications
- Corriger les modifications (faire des commits)
- Soumettez votre version sur votre GitHub
- Sur le site GitHub, appuyez sur le bouton **pull request**
***