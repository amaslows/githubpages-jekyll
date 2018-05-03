---
title: "Initial Post"
date: 2018-05-02
---
## Basic GIT workflow

I'm glad you are here. I plan to talk about basic git flow:

### Clone Repo
- git clone `<url>`
- cd `<reponame>`

### Create new feature branch
- git checkout -b `<branchname>`

## Merge with master to ensure in sync and make the change
- git merge master
- vi `<filename>`

## Add the files and commit the code
- git add . (or git add -u to remove deleted files, or git add --all for all adds and deletes)
- git commit -m "message in present tense"

## Push the new branch to github
- git push -u origin `<branchname>`

## Merge the code to the master (ensuring you have all latest code from remote repo first)
- git checkout `<branchname>`
- git pull origin `<branchname>`
- git pull origin master
- git checkout master
- git pull origin master
- git merge --no-ff `<branchname>`

## Delete the branches now that the merge is complete and they are no longer needed
- git push origin --delete `<branchname>`
- git branch -d `<branchname>`

