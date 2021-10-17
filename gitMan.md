# Create a Repository or Initialize Git in folder
git init

# Add Files
git add . #All Files
git add <filename> ##Single File

# Commit the Changes
git commit -m "first commit"

# Remote Repository
git remote add "Remote Name" <link from github>
git remote add origin https://github.com/samytech/New-Projects.git  (Git Address with .git in the end)

# View Remote Branches 
git remote -v 

# Pull updated files from branch
git pull <remote_name> <branch_name> 
git pull pro master

# Remove Remote branch from local
git remote remove <branch_name>  ==>  The git remote remove command removes a remote from a local repository.
git remote rm <branch_name> ==> You can use the shorter git remote rm command too.

# Final Step (Push in Master Branch)
git push -u origin master

# Check changes 
git status

# Check Git Log
git log

## CREATE BRANCH ##

# Show Branches
git branch  #show local branches
git branch -a   #show both local and server branches [Server branches in Red color]

# Create & checkout Branhc
git branch <branch_name> 
git branch develop  ==> it creates new branch named 'develop' but still keep being on master branch
git checkout develop ==> it will change your branch to the develop branch
git checkout -b develop ==> it creates also a branch named develop and switches to it automatically

# Delete Branch
git branch -d <branch_name> ==> deletes the branch. If we have unmerged changes, this command gives a warning and does not delete.  
git branch -D <branch_name> ===> deletes the branch even if it has unmerged changes. It gives no warning.

# Merge Branch
git merge <branch_name>  ==>  this command takes changes from the given branch, and merges with the current branches we are on. 