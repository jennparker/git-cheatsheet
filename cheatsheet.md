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

### Cherry pick a commit
git cherry-pick <revision number>

### Move most recent X commits back to staging
git reset --soft HEAD~X

### Revert all local changes
git reset --hard

### List of all available local branches
git branch

### List of all branches in the repo
git branch -r

### List upstream branch for each local branch
git branch -vv

### Create a new remote branch and push commit from current working branch
git push --force origin HEAD:cool-name

### Show the contents of the most recent stash
git stash show -p

### Rename a branch (from that branch)
git branch -m new-name

### Change commit message on local commit
git commit --amend -m "New commit message"

### Add additional file to a commit
git commit --amend --no-edit

### Push repo Develop to repo Master
git checkout master 
git merge develop
git push -u origin master

### Create a local branch from an existing remote branch
git checkout -b your-witty-and-creative-local-name-for-remote (e.g. create a new local branch and name it whatever you want)
git pull origin name-of-remote

