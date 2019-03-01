# GEN_labo1

Auteurs: Pierre Kohler, Jonathan Zaehringer 


## Commandes exécutées afin d'obtenir le bon *network*

```bash
# clonage du repo (avec le commit initial uniquement)
git clone git@github.com:jzaehrin/GEN_labo1.git
cd GEN_labo1

# master1
touch master1
git add .
git commit -m "master1"
git push

# création de la branch essai
git branch essai
git checkout essai

# essai1
touch essai1
git add .
git commit -m "essai1"
git push --set-upstream origin essai

# essai2
touch essai2
git add .
git commit -m "essai2"
git push

# essai3
touch essai3
git add .
git commit -m "essai3"
git push

# master2
git checkout master
touch master2
git add .
git commit -m "master2"
git push

# merge essai2 -> master
git checkout essai
git checkout master
git merge 511349a
git push

# essai4
git checkout essai
touch essai4
git add .
git commit -m "essai4"
git push

# branch à supprimer plus tard
git checkout master
git branch deleted
git checkout deleted
touch deleted1
git add .
git commit -m "deleted1"
git push --set-upstream origin deleted

# merge essai -> master
git checkout master
git merge essai
git push

# création de la branch dev
git checkout 511349a
git branch dev
git checkout dev

# dev1
touch dev1
git add .
git commit -m "dev1"
git push --set-upstream origin dev

# création de la branch essai3
git branch essai3
git checkout essai3

# essai31
touch essai31
git add .
git commit -m "essai31"
git push --set-upstream origin essai3

# suppression de la branch deleted
git checkout master
git merge deleted
git push
git branch -D deleted
git push --delete origin deleted
```
