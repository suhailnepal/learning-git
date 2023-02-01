## Git commands

This page will have a list of Git commands which I use/intend to use on a daily basis. For commands which are new to me, I will write up a short description on what it does in the background:

* git push --set-upstream origin branchname
* git remote -v
The above command will let you view origin (remote repository)
* git config --list --show-origin
* git checkout {branchname}
The above command will change branch on the repo, it doesn't create a new branch.
* git checkout -b {branchname}
The above command will create a new branch and will also change the branch.
* git checkout {filename}
The above command will discard changes from an existing file in the repo.
* git branch -d {branchname}
The above command will delete the branch (manually)
* git branch -a
The above command will list down all the branches in the repo. 
Ensure that you done a `git fetch` on the repo which will fetch all the remote branches in the repo. 
* git log
* git log --all --graph --oneline --decorate 
The above command will make the logs look a bit cleaner.
* git commit --amend
The above command will amend the last commit message, it will open up a new terminal where you can make changes. 
