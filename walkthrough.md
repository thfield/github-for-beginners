# Walkthrough
## The Basics
1. Create the repo on Github
1. Make a local copy
  - `$ git clone {url}`
1. Add some files
  - `$ touch foo.txt`
  - `$ git add foo.txt`
1. Commit
  - `$ git commit -m "Initial commit"`
1. Make some changes and commit
  - `$ echo "bar" >> foo.txt`
  - `$ git status`
  - `$ git add -u`
  - `$ git commit -m 'add some content'`
1. See the history of changes
  - `$ git log`
1. Push local changes to Github
    -`$ git push`

## Branch and Merge
1. Make a branch
  - `$ git branch neato-feature`
  - `$ git checkout neato-feature`
1. See which branches are available
  - `$ git branch`
1. Make some changes
  - `$ echo "asdfasdf" >> foo.txt`
  - `$ git commit -am 'add to the content'`
1. Merge the branch
  - `$ git checkout master`
  - `$ git merge neato-feature`
1. Delete the old branch
  - `$ git branch -d neato-feature`
1. Push local changes to Github
    -`$ git push`

##  Parallel Development
1. Pull from upstream; the repos are the same
1. Make some changes
  - `$ echo "qwertyuiop" >> foo.txt`
  - `$ git commit -am 'add qwerty`
1. The repo gets changed upstream
1. Push local changes to Github - Uh Oh!
  - `$ git push`
1. Bring in upstream changes
  - `$ git pull`
1. Resolve any conflicts
 - `$ git commit`
1. Push to Github
  - `$ git push`

## Stashing
1. Do some work, not quite ready for a commit.
1. Check out another branch to examine changes.
1. Whoops!
  - `$ git stash`
1. Now your changes are stashed away, you can checkout the branch.
1. Ready to start working again?
  - `$ git stash apply`

[<-Previous](git.md)