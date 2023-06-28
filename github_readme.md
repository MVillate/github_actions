
create a new empty project 
git remote add origin https://github.com/MVillate/github_actions.git
git push # this will fail

The origin has been added, but not linked to the local branch. for that is necessary
git push -u, --set-upstream

git push -u origin main


checking the remote 
git remote -v

git remote remove origin




git remote add origin https://${GITHUB_USER}:${GITHUB_TOKEN}@github.com/MVillate/github_actions.git

git remote add origin https://${GITHUB_TOKEN}@github.com/${GITHUB_USER}/${GITHUB_REPO}.git
git remote add origin https://${GITHUB_TOKEN}@github.com/${GITHUB_USER}/github_actions.git
