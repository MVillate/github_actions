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