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
> git branch branch5  
> git checkout branch5  
> vi README.md  
> git commit -am 'branch branch5'  
> git push -u origin branch5  

## fast-forward merge to master
> git checkout master  
> git merge branch5  

## create branch for continued work today
> git branch branch5.b  
> git checkout branch5.b  
> vi README.md  
> git commit -am 'branch branch5.b'  
> git push -u origin branch5.b  

## abandon branch branch5.b
> git checkout master  
> vi README.md  
> git commit -am 'abandoned branch5.b'  
> git push -u origin master  

## changed mind, merging branch branch5.b
> git merge branch5.b  
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
_display hashes of previous commits_  
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
