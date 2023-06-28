
create a new empty project 
git remote add origin https://github.com/MVillate/github_actions.git
git push # this will fail


## Adding the origin

For personal repositories
```
git remote add origin https://${GITHUB_TOKEN}@github.com/${GITHUB_USER}/${GITHUB_REPO}.git
```

For corporate repositories
```
git remote add origin https://${GITHUB_USER}:${GITHUB_TOKEN}@github.com/${GITHUB_ORGANIZATION}/{GITHUB_REPO}.git
```

## Linking the origin with the local branch
The origin has been added, but not linked to the local branch. To link the origin with the 
git push -u, --set-upstream
```
git push -u origin main
```
Once the origin has been linked, it's enough with git push

## Status of the origin
git remote -v
git remote remove origin


