# Git
## Branches
### Creating branches
Create a branch
```
git branch [new branch]
```
Checkout the new branch
```
git checkout [new branch]
```
Create a new branch and check it out in one command
```
git checkout -b [new branch]
```
### Deleting branches
Delete a local branch
```
git branch -d [branch name]
```
Delete a local branch even if it hasn't been fully merged
```
git branch -D [branch name]
```
Delete a branch on a remote
```
git push --delete [remote name] [branch name]
```
Older versions of GIT have a different syntax for deleting remote branches
```
git push [remmote name] :[branch name]
```

### Pruning remotes
Remove tracking for deleted remote branches
```
git remote prune [remote name]
```

### Merging branches
Merge master into a feature branch
```
git checkout [feature branch name]
git merge master
```
Using the no fast forward option brings in all commits and does not create a merge commit.  Only useful if there has been no activity in the feature branch since it was originally created.
```
git merge --no-ff master
```

