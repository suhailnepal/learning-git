## Git commands

This page will have a list of Git commands which I use/intend to use on a daily basis. For commands which are new to me, I will write up a short description on what it does in the background:

* git push --set-upstream origin branchname
* git remote -v
(This command will let you view origin (remote repository))
* git config --list --show-origin
* git checkout {branchname}
(This command will change branch on the repo, it doesn't create a new branch.)
* git checkout -b {branchname}
(This command will create a new branch and will also change the branch.)
* git checkout {filename}
(This command will discard changes from an existing file in the repo.)
* git branch -d {branchname}
(This command will delete the branch (manually))
* git branch -a
(This command will list down all the branches in the repo.)
Ensure that you done a `git fetch` on the repo which will fetch all the remote branches in the repo. 
* git log
* git log --all --graph --oneline --decorate 
(This command will make the logs look a bit cleaner.)
* git commit --amend
(This command will amend the last commit message, it will open up a new terminal where you can make changes.)
* git reset --soft HEAD~1
(This command will reset the last commit message, soft reset will ensure that any files which are not commited or tracked will remain as is.)
* git config --global fetch.prune true
(This git config will ensure that all branches which are not being used will be pruned or cleaned. Be cautious before using this command.)
* git config --global pull.rebase true
(This git config will ensure that all git pull moving forward will do a rebase with all git pull)
