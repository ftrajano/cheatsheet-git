# cheatsheet-git
A git cheatsheet to help me remembering git commands.
---
## Basic Commands
+ **git log**: show the list of commits made.
+ **git show hashcode**: show details of specific commit.
+ **git show HEAD~3**: show details of the last 4th. commit.
+ **git annotate file_name**: show the changes in the files, line by line, per commit as the author, time, line and line content.

## Undoing changes before a commit
+ **git reset HEAD filename**: unstage a specific file. 
+ **git reset HEAD**: unstage all files.

## Undo changes to an unstaged file
* **git checkout -- filename**: checkout to a previous commit version of the file. (Checkout means switching to a different version).
* **git checkout .**: Undo changes to all unstaged files in the current directory.


## Viewing changes
* **git diff -r HEAD**: show differences in staged files and commit
* **git diff -r HEAD~1**: show differences in the second last commit
* **git diff name_of_file**: show differences between the non-staged file and the last commit
* **git diff hashcode1 hashcode2**: show difference between commits
* **git diff HEAD~2 HEAD~3**: same as above.

## Backtrack in git
* **git checkout HEAD filename**: Discards changes in the working directory.
* **git reset HEAD filename**: Unstages file changes in the staging area.
* **git reset commit_SHA**: Resets to a previous commit in your commit history.


## Git Teamwork
* **git clone remote_location clone_name**
* **git clone**: Creates a local copy of a remote.
* **git remote** -v: Lists a Git project’s remotes.
* **git fetch**: Fetches work from the remote into the local copy.
* **git merge origin/master**: Merges origin/master into your local branch.
* **git push origin <branch_name>**: Pushes a local branch to the origin remote.
