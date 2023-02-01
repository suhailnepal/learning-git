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

