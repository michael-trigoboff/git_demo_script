# GitHub Demo

## create repository on github
> _will use listed command to connect local directory to this repository_

## create local repository
> md git_demo  
> git init  
> vi README.md  
> git status  
> git add README.md  
> git commit -am 'first'  

## connect to GitHub repository
> git remote add origin https://github.com/michael-trigoboff/git_demo.git  
> git push -u origin master  

## create branch for today's work
> git branch 11/12  
> git checkout 11/12  
> vi README.md  
> git commit -am 'branch 11/12'  
> git push -u origin 11/12  

## fast-forward merge to master
> git checkout master  
> git merge 11/12  

## create branch for continued work today
> git branch 11/12.b  
> git checkout 11/12.b  
> vi README.md  
> git commit -am 'branch 11/12.b'  
> git push -u origin 11/12.b  

## abandon branch 11/12.b
> git checkout master  
> vi README.md  
> git commit -am 'abandoned 11/12.b'  
> git push -u origin master  

## changed mind, merging branch 11/12.b
> git merge 11/12.b  
_merge conflict!_  

## fix conflict
> vi README.md  
> git commit -am 'fixed conflict'  
> git push -u origin master  

## pull change from server
> git pull

## change file, abandon change by going back to previous commit
> vi README.md  
> git checkout -- README.md

## get version of file from previous commit
> _display hashes of previous commits_  
> git log --stat  
> git checkout <commit_hash> README.md  

## display remote repositories
> git remote  
> git remote -v  

## add remote repository  
> git remote add <short_name> <repo_url>

## rename remote (i.e. change short_name)
> git remote rename <old_short_name> <new_short_name>  

## remove remote
> git remote remove <short_name>  

## clone remote repository to empty directory (without creating subdirectory)
> git clone <repository_url> .  
