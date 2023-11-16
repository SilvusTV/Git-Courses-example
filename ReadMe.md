# Etapes à suivre :
Voici la liste des commandes qui ont été faites :

- git init "ProjetVersGITHUB" \
  &nbsp;\
Context : add `.gitignore` and `ReadMe.md` files | add `.idea/` on `.gitignore` | prepare documentation on `ReadMe.md`
- git add .
- git ci -m "Init Project" \
  &nbsp;\
Context : update documentation on `ReadMe.md` (visual and comprehension)
- git add ReadMe.md
- git ci -m "Update readMe.md for project init"\
  &nbsp;\
Context : Prepare first web pages and all necessary files (css, html)
- git add .
- git st
- git rm --cached style.css
- git st
- git ci -m "add index.html"\
  &nbsp;\
  Context : ...
- git add . 
- git st
- git ci -m "add style.css"\
  &nbsp;\
  Context : oublie de link le css à l'html.
- git add .
- git st
- git ci --amend -m "add css link on html"\
  &nbsp;\
  Context : Creation d'une nouvelle branche pour la tentative de création d'un affiché caché + html.
- git co -b "affichéCaché"
- git add .
- git ci -m "HTML affiché caché"\
  &nbsp;\
  Context : Ajoue du CSS à l'affiché caché .
- git add .
- git ci -m "Ajoue du css"\
  &nbsp;\
  Context : fonctionnalité fini alors merge dans master et suppression de la branche actuelle.
- git add .
- git ci -m "update ReadMe.md"
- git co master
- git merge affichéCaché
- git branch -d affichéCaché\
  &nbsp;\
  Context : Connect local Project on GitHub, create remote gitHub repository.
- git remote add origin https://github.com/SilvusTV/Git-Courses-example.git
- git remote -v
- git push --set-upstream origin master\
  &nbsp;\
  Context : edit `ReadMe.md`.
- git add .
- git ci -m "update last time readme.md"
- git push