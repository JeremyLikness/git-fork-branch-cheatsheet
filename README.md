# git-fork-branch-cheatsheet

My cheat sheet for the git/fork/branch workflow.

## Set up

1. Fork it
2. `git clone <forked repo>`
3. `git remote add upstream <original repo>.git`

## Workflow

1. `git pull upstream master`
2. `git push origin master`
3. `git checkout -b <branch>`
4. Work. Work. Work.
5. `git push origin <branch>`
6. Create PR
7. Wait for it to be merged, then ...
8. `git checkout master`
9. `git pull upstream master`
10. `git branch -d <branch>` (or `-D` if necessary)
11. `git push origin master`
12. `git push --delete origin <branch>`
13. `git pull upstream master`
14. `git push origin master`

## Get out of Jail, Free

(when things go wrong, force fork to sync with upstream)

1. `git fetch upstream`
2. `git reset --hard upstream/master`
3. `git push origin master --force`

_quod erat demonstrandum_

