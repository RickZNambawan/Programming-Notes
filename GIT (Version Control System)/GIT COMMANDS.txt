* git <keyword here> -h
= to look for the manuals of the keyword

* git --version 
= to know what version of the git installed.

* git config --global user.name "name here"
* git config --global user.email "email here"
= to create your own username and email

* git config user.name "name here"
* git config user.email (email here)
= to override with diff name, diff email for specific project

* git config --global core.editor "full path of text editor"
= to set your default text editor

* git config --list
= to check all the lis of configuration values you have

* git config --global alias.(name you want to replace) (keyword)
= to modify the keyword

* touch .gitignore
= to create file that can ignore the unneccessary files
  you don't want to include to repository
= put name of the file

* touch (name of the file with extension)
= to create file to that directory

* echo 'text you want to put' > (name of the file)
= to create a file with text inside

* ls
= to show all the files that are visible without some details.

* ls -la 
= to check all the files within the directory with hidden files and some details.

* cd ..
= to back from the previous directory

* cd (Folders/folder) 
= to go to that directory

* rm (name of the files/folder)
= to delete files from Git directory and will go to unstaged area.

* rm -rf (name of the file/folder)
= to force delete the file

* git init
= to create a folder and to track the repository

* git status
= to show the status of all the changes

* git status -s
= to show the changes in a compact way

* git add (files) = add one by one
* git add -A = add all files
* git add . = add all files 
= to add files to the staging area

* git commit -m "message here"
= to commit all changes from the staging area

* git commit -a -m "message here"
= to skip staging area and commit all changes without git add except untracked files.

* git commit --amend -m "message"
= to overwrite your last commit message

* git reset --soft (hash of before the commit)
= to reset the commited file that has been made but ready to commit.

* git reset (hash of before the commit)
= to reset the commit that has been made to unstage.

* git reset --hard
= to reset all changes/files from staging area and unstaged except untracked files.

* git clean -df
= to delete all files that are on untracked files.

* git reset (name of the files)
= to reset one by one the file from staging area to unstage.

* git reset
= to reset all file from staging area to unstage.

* git checkout (name of the file)
= to reset all changes from that file

* git mv (name of the file) (name you want to change)
= to rename the file

* git reflog 
= to see all the list of changes have been made.

* git log
= to see the commits that was made

* git log -p
= to see the commits and diff of the changes

* git clone (URL remote or Directory path for local) .
= to download or make a clone of the files of other repository

* git clone (URL remote or Directory path for local) (modified name of the folder)
= to rename the remote repository folder before cloning it.

* git diff
= to see what changes you've made before staging it.

* git diff (branch)
= to see what changes you've made to that branch.

* git diff --staged
= to see what changes you've made to the staged area.

* git diff (first hash) (second hash)
= to see the changes of the two files

* git remote
= to show the list of names of the remote repository

* git remote (name of the remote) (name you want to change)
= to rename your remote repository

* git remote -v
= to show the list of name and link/path of remote repository

* git remote remove (name of the remote repo)
= to remove existing remote repo

* git branch (name of the branch)
= to create new branch

* git checkout (name of the branch)
= to go to your desire branch

* git checkout -b (name of the branch)
= to create new branch and automatically go to that branch

* git merge (name of the branch)
= to merge the specific branch to the master branch

* git branch -d (name of the branch)
= to delete the branch

* git push origin --delete (name of the branch)
= to delete the branch from remote repo using clone repo

* git push origin (name of the branch)
= to push the branch to the remote repository

* git fetch origin
= to check the past push commits before merging/pulling commits

* git diff master origin/master
= to show the changes or past commits before merging/pulling commits

* git pull origin (name of the branch)
= to pull the commits that changed from the remote repo and branch

* git push origin master
= to push all the changes you've made from your local repo to remote repo origin, master branch

* git pull origin master
= to pull all the changes that other have made from remote repo origin, master branch, to your local repo



** BRING BACK CHANGES/FILES **

-- See the list of changes you want to back --
-- Grab the hash of the history from git reflog--
* git reflog

-- Paste the hash to bring back the reset file.
* git checkout (hash)

-- Create new branch backup to store the changes --
* git branch (name of the branch)

-- And then go to other branch to save the changes --
* git checkout master



** STASHING CHANGES **

* git stash save "message here"
= to save your changes in stash 

* git stash list
= to show the list of stash

* git stash pop (name of the stash@{})
= to remove changes from stash

* git stash clear
= to remove all changes from stash



** TO ADD CHANGES TO THE COMMITED FILES **

-- After commited and if you want to add changes to the commited files --
-- Add the files you want to add to the commited files --
* git add -A

* git commit --amend

-- Then press esc key and type :wq to exit from interactive shell --
-- DONE --



** TO CREATE NEW REPOSITORY AND PUSH TO REMOTE REPOSITORY **

-- Create your local repository --
* git init

* git remote add origin (URL of your github account)

* git push -u origin (name of your branch)



** TO PUSH EXISTING REPOSITORY FROM LOCAL TO REMOTE REPOSITORY **

* git remote add origin (URL of your github account)

* git push -u origin (name of the branch)



** COMMON WORKFLOW **

* git fetch origin

* git diff master origin/master

* git pull origin master 