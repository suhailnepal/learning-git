## Notes

I will try to uncover some terminologies and concepts on this page: 

### Upstream and downstream

Think of upstream as the source and downstream as the destination in github. For example if you are working on a repo and trying to fork from another remote repo, your working repo is downstream is the repo from which you are forking from is your upstream. 

This is very common in the following, here branch1 is the name of the branch 
`git push --set-upstream origin branch1`

### Head

Head is a pointer which tells us where the current branch is pointing. The other way to look at this, it tells us where we are working at the moment.

### Gitignore

This is a file which can used if you want to ignore a specific file to be commited. You can use regex, wildcards in gitignore. One of the example could be with terraform where you don't want to commit *.tfstate file and might want to add them in .gitignore files.

### Git pull

At a very high level, there are 2 ways of doing a git pull:
* git pull --rebase
* git pull --ff-only
In the above, ff stands for fast forward merge which is the default way of doina a merge, it is recommended to use the first method for git pull, you can add the following in your git config to ensure that rebase is the chosen method for all git pulls
* git config --global pull.rebase true

### Rebase from another branch

This is a very common scnerio where you are working on a new branch and want to rebase with master before you create a PR. I have had this situation where I had had to work on a branch for few days, and there was a delta of changes in the main branch during those time. 
Run the following commands in sequenuce so that you are branch is upto date before merging/creating a PR:

* git checkout {branch}
* git fetch origin main
* git rebase origin/main
