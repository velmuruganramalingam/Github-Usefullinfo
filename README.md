# Github-Usefullinfo

## To revert the changes done to the local working directory
Git checkout .


## GIT Reset command
There are 3 kinds of files Staged,Tracked and UnTracked
* Type 1. Staged Tracked files
* Type 2. Unstaged Tracked files
* Type 3. Unstaged UnTracked files a.k.a UnTracked files

* Staged - Those that are moved to staging area/ Added to index
* Tracked - modified files
* UnTracked - new files. Always unstaged. If staged, that means they are tracked.

## What each commands do:
* **```git checkout .```** - Removes Unstaged Tracked files ONLY [Type 2]
* **```git clean -n```** - shows the list of untracked files that will be deleted
* **```git clean -f```** - Removes Unstaged UnTracked files ONLY [Type 3]
* **```git reset HEAD <file_name>```** - Moves the file from Staged to Unstaged
* **```git reset --hard```** - Removes Staged Tracked and UnStaged Tracked files ONLY[Type 1, Type 2]
* **```git stash -u```** - Removes all changes [Type 1, Type 2, Type 3]



## Create review branch
    rake translations:generate  
    git checkout master  
    git status                      #To check nothing is checked out in master
    git pull  
    git checkout -b <review_branch>  
    git merge --squash <dev_branch>  
    git add .  
    git commit -am "<comments>"  
    git push origin <review_branch>  

## Merging from master into development branch
    git checkout master         |
    git status                  | #To check nothing is checked out in master
    git pull                    |
    git checkout <dev_branch>   |
    git merge master            |  git fetch origin && git merge origin/master 
    <resolve conflicts in files>  
    git status
    git add .  
    git commit -m “<comments>”  
    git push origin <dev_branch>  
## Merging from development branch into master
    rake translations:generate  
    git checkout master 
    git status                     #To check nothing is checked out in master
    git pull  
    git merge —squash <dev_branch>   
    rake site 
    check for lints, translations and test cases  
    git status  
    git add .  
    git commit -m “<comments>”  
    git push  
 ## Git Stashing
    git stash  
    git stash apply  
    git stash list  
    
 ## Delete branches
     git push origin --delete <branch_name>  
     git push origin :<branch_name>  
