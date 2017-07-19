# Github-Usefullinfo

## To revert the changes done to the local working directory
Git checkout .


## GIT Reset command
There are 3 kinds of files Staged,Tracked and UnTracked
Type 1. Staged Tracked files
Type 2. Unstaged Tracked files
Type 3. Unstaged UnTracked files a.k.a UnTracked files

Staged - Those that are moved to staging area/ Added to index
Tracked - modified files
UnTracked - new files. Always unstaged. If staged, that means they are tracked.

## What each commands do:
* **```git checkout .```** - Removes Unstaged Tracked files ONLY [Type 2]
* **```git clean -f```** - Removes Unstaged UnTracked files ONLY [Type 3]
* **```git reset --hard```** - Removes Staged Tracked and UnStaged Tracked files ONLY[Type 1, Type 2]
* **```git stash -u```** - Removes all changes [Type 1, Type 2, Type 3]
