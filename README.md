new_repo
========

mkdir new_repo
cd new_repo/

git init

echo "New Repo" > dummy
git add .
git commit -m "Initial commit"

git remote add -f gittest1 git@github.com:patrox/gittest1.git
git merge gittest1/master

git rm dummy
git commit -m "clean up dummy file"

mkdir gittest1

git mv module1 README.md gittest1
git commit -m "Move gittest1 files into a subdir"

git remote add -f gittest2 git@github.com:patrox/gittest2.git
git merge gittest2/master

mkdir gittest2
git mv dir2 dir3 gittest2
git commit -m "Move gittest2 files into a subdir"

git remote add new_repo git@github.com:patrox/new_repo.git
git push -u new_repo master
