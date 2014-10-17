new_repo
========

```bash
mkdir new_repo
cd new_repo/
```

```bash
git init
```

```bash
echo "New Repo" > dummy
git add .
git commit -m "Initial commit"
```

```bash
git remote add -f gittest1 git@github.com:patrox/gittest1.git
git merge gittest1/master
```

```bash
git rm dummy
git commit -m "clean up dummy file"
```

```bash
mkdir gittest1
```

```bash
git mv module1 README.md gittest1
git commit -m "Move gittest1 files into a subdir"
```

```bash
git remote add -f gittest2 git@github.com:patrox/gittest2.git
git merge gittest2/master
```

```bash
mkdir gittest2
git mv dir2 dir3 gittest2
git commit -m "Move gittest2 files into a subdir"
```

```bash
git remote add new_repo git@github.com:patrox/new_repo.git
git push -u new_repo master
```
