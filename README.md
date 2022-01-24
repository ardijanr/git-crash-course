# Git crash course cheat-sheet


## Common commands:
Pull changes from remote
```
git clone <remote repo link> <folder name>  
```
\
Check the state of your github repo
```
git status
```
\
Commit changes
```
git commit -a -m "<commit message>"
```
\
Make git track all new changes to the git repo. 
All new changes also means new files etc. Make sure your gitignore file is properly set up.
```
git add -A
```
\
Push your changes to the remote
```
git push
```
\
Pull changes from remote
```
git pull
```
## Branches

Make a new branch
```
git branch <branch name>
```
\
See all branches, and which one you are working in.
```
git branch -a
```
\
Push local branch to remote
```
git push -u <remote> <branch name>
```
\
Make a new branch and move into it
```
git checkout -b <branch name>
```
\
Merge \<branch name\> into current branch
```
git merge <branch name>
```
\
Delete branch locally
```
git branch -d <branch name>
```
\
Delete remote branch
```
git push origin --delete <branch name>
```





## Other Commands 
View remote
```
git remote -v
```
\
Go back to previous commit
```
git checkout <commit hash>
```

## Potentially dangerous commands

Force push remote
```
git push -f
```
\
Delete all local changes
```
git reset --hard HEAD
```
\
Reset current branch to another branch/remote branch
```
git reset --hard <remote>/<branch_name>
```

