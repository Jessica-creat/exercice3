1. Créer un nouveau repository Git
git init
2. Ajouter un fichier et le commiter `(C1)`
touch fichier.txt
git add .
git commit -m "Ajout du fichier.txt"
3. Modifier la première ligne du fichier et commiter `(C2)`
git status
git add .
git commit -m "Modification de la première ligne du fichier"
4. Créer une feature branch `B1` à partir de `C1`
git log --oneline
git checkout 64d6c67
git checkout -b B1
5. Faire une modification de la première ligne du fichier et commiter `(C3)`
git add fichier.txt
git commit -m "Modification de la première ligne dans B1"
6. Merger `B1` dans `main` ou `master` en résolvant les conflits
git checkout master
git merge B1
