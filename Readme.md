# GIT CRASH COURSE

## Configuring GIT
git config --global user.name "your-username"
git config --global user.email "your-email"

## Initializing
git init

The initial branch will be called master. To rename it as main

git branch -m main

## Status
git status
git log 

From git log we get the information about HEAD: (HEAD -> main)
HEAD is a pointer that points at the commit that is currently loaded/visible.

## Commits (snapshots)

### Staging the changes
git add {{ file }}
git add {{ file1 }} {{ file2 }}
git add . 

### Unstaging 
git restore --staged {{ file1 }}
git restore --staged {{ file1 }} {{ file1 }}
git restore --staged .

### Creating commits
git commit -m {{ message }}

### Move between commits
git checkout {{ id }} - Temporarily move to another commit
git checkout main - To return to the latest commit in main

## Reverting
git revert {{ id }} 
This Id is the last change you want to revert from. 
This will add a new commit identical as the previous to last
By default it adds a message saying Revert "{{ commit message of the last commit }}"
It keeps all the commits in the commit history

## Resetting 
git reset --hard {{ id }}
This ID is the commit you want to go to, and everything after that will be deleted. 
This removes part of the history

## Branches
Containers that contain commits

git branch {{ branch_name }} - creates branch
git branch -D {{ branch_name }} - deletes the branch
git checkout {{ branch_name }} - moves to the new branch

git checkout -b {{ branch_name } - creates branch and checksout branch}

git branch - Lists the branches