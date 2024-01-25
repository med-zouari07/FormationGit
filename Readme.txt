Commit : capture les commit que vous avez fait dans votre projet à l’instant t : pour suivre votre historique 

First Step after installing git : 

git config —global [user.name](http://user.name) “<votre nom>”

git config —global [user.](http://user.name)email “<votre mail>”

1/ git init : pour initialiser un noveau projet 

2/ git add .  : ajouter tous les fichiers et les noveaux

3/ git commit -m “premier commit”

4/git remote add origin <URL_du_dépot distant> : to Link project in local to project in github  

5/git push -u <origin> master

6/ git clone https://github/utilisateur/nom du depot.git nom-du-depot-local  VIA HTTPS

6/* git clone git@github.com:utilisateur/nom-du depot.git nom-du-depot-local

SSH : 

** verify the SSH existant  : 

ls -al -/.ssh 

** Generate for private & public key :

Add  the key SSH : 

1-

ssh-keygen -t rsa -b 4096 -c “votre@email.com”

2- add the key SSH to the Agent SSH

eval “$(ssh-agent -s)”

3- Add the public key to you account Github 

cat ~/.ssh/id_rsa.pub