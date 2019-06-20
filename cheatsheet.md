# Git Cheatsheet

### Set upstream branch
git branch --set-upstream-to=<branch to track>

### Force push 
(use this to squash and repush already pushed branches)
1) Squash the commits locally
2) git push --force origin HEAD:banner

### Push only one of multiple local commits
1) Interactive rebase to make the desired commit first on the list
2) git push origin <commit sha>:banner

### Move most recent X commits back to staging
git reset --soft HEAD~X

### List of all available local branches
git branch

### List of all branches in the repo
git branch -r

### List upstream branch for each local branch
git branch -vv

### Create a new remote branch and push commit from current working branch
git push --force origin HEAD:cool-name
