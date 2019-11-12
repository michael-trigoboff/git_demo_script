# GitHub Demo

## create repository on github
> _will use listed command to connect local directory to it_

## create local repository
> md git_demo_gh  
> cd git_demo_gh  
> git init  
> cp ../start_git/README.md .  
> vi README.md  
> git status  
> git add README.md  
> git commit -a -m 'first'  

## connect to GitHub repository
> git remote add origin https://github.com/michael-trigoboff/git_demo_gh.git  
> git push -u origin master  

## create branch for today's work
> git branch 11/12  
> git checkout 11/12  
> vi README.md  
> git commit -a -m 'branch 11/12'  
> git push -u origin 11/12  

## fast-forward merge to master
> git checkout master  
> git merge 11/12  

## create branch for continued work today
> git branch 11/12.b  
> git checkout 11/12.b  
> vi README.md  
> git commit -a -m 'branch 11/12.b'  
> git push -u origin 11/12.b  

## abandon branch 11/12.b
> git checkout master  
> vi README.md  
> git commit -a -m 'abandoned 11/12.b'  
> git push -u origin master  

## changed mind, merging branch 11/12.b
> git merge 11/12.b  
_merge conflict!_  

## fix conflict
> vi README.md  
> git commit -a -m 'fixed conflict'  
> git push -u origin master  
