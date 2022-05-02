# Test Repo - for training purpose only

## BEGIN

### General info

```bash
git status
git log         // see commits on branch
git branch      // see branches
git remote -v   // see remote url
```

### Create new repo

```bash
echo "# Git-test" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin git@github.com:Peanuts-83/Git-test.git
git push -u origin main  // -u = --set-upstream
```

### Push an existing repo

```bash
git remote add origin git@github.com:Peanuts-83/Git-test.git
git branch -M main
git push -u origin main
```

### Import code from another repo

```bash
git clone git@github.com:Peanuts-83/Git-test.git
// or add repo in another repo
git submodule add git@github.com:Peanuts-83/Git-test.git
```

### Commit all & push

```bash
git add .
git commit -m'Name of the commit'
git push
```

## BRANCHES

### Create branch & go on it

```bash
git branch branchName
git checkout branchName
// or short command
git checkout -b branchName
```

### Copy branch or commit under HEAD

Originals remain the same

```bash
git cherry-pick branch1 branch2 de9a6fb // branch or commit names
```

### Merge branch

Merged branch ends to merge point. It comes to HEAD.
```bash
git merge branch2
```