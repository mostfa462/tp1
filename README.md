1)Vérifier le nom d'utilisateur :



git config --global user.name

2 )Vérifier l'adresse e-mail :



git config --global user.email

 3) Vérifier toutes les configurations globales de Git :



git config --global --list

4) modifier l'adresse mail : 
git config --global user.email "votre.nouvelle.adresse@example.com"


5. Ajouter des fichiers à l'index (staging)

Si vous avez des fichiers que vous souhaitez committer, ajoutez-les à l'index avec :


git add nom_du_fichier

Ou pour ajouter tous les fichiers modifiés :

bash

git add .

6. Commettre les changements

Ensuite, effectuez le commit :

bash

git commit -m "Votre message de commit décrivant les changements"

7. Pousser les changements vers le dépôt distant (si nécessaire)

Enfin, si vous souhaitez envoyer vos modifications vers le dépôt distant, utilisez :

bash

git push origin nom_de_branche




8. Créer un dépôt distant



Naviguez vers le répertoire de votre projet avec le terminal :

bash

cd /chemin/vers/votre/projet

9. Ajouter le dépôt distant

Utilisez la commande suivante pour ajouter le dépôt distant :

bash

git remote add origin https://github.com/username/repository.git

Remplacez l'URL par celle de votre dépôt.
. Vérifier la configuration des dépôts distants

Pour vous assurer que le dépôt distant a été ajouté correctement, exécutez :

bash

git remote -v

Cela affichera la liste des dépôts distants configurés. Vous devriez voir une sortie indiquant l'URL que vous venez d'ajouter.
 Pousser vos changements

Si vous avez des commits locaux que vous souhaitez envoyer vers le dépôt distant, utilisez :

bash

git push -u origin main


Annuler les modifications locales

Si vous souhaitez réinitialiser un fichier à son état dans le dernier commit, utilisez :

bash

git checkout -- nom_du_fichier

 Comment visualiser les fichiers qui sont prêts à être commités dans Git (staging) ?
git diff --cached
Comment suivre (track) un dépôt distant et récupérer toutes les branches de ce dépôt ?
git fetch origin

Comment supprimer une branche locale après l'avoir fusionnée dans master ?


git branch -d nom_de_branche

Comment interrompre un rebase en cours si vous avez commis une erreur ?
git rebase --abort

Comment lister les commits qui vont être rebasés avant de lancer un rebase ?
git rebase -i master

Comment afficher la liste des branches ac�ves et en cours de développement dans
Gi�low ?
git flow feature list

Comment annuler une branche de correc�f (ho�ix) avant de la finaliser si vous constatez
une erreur ?

git flow hotfix abort


