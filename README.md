# git-fork-branch-cheatsheet

My cheat sheet for the git/fork/branch workflow.

## Set up

1. Fork it
2. `git clone <forked repo>`
3. `git remote add upstream <original repo>.git`

## Workflow

1. `git pull upstream master`
2. `git push origin master`
3. `git checkout -b branch`
4. Work. Work. Work.
5. `git push origin branch`
6. Create PR
7. `git pull upstream master`
8. `git branch -d branch` (or `-D` if necessary)
9. `git push origin master`
10. `git push --delete origin branch`
11. `git pull upstream master`
12. `git push origin master`

_quod erat demonstrandum_

