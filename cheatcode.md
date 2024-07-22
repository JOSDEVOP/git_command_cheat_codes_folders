```markdown

# How to master Git and Github 


Git is software that is installed locally on your computer and can be used as for version controlling all kinds of works like writing and writing codes .
Github is the remote place where one can collaborate and word on repos stored on the cloud.

-- To install git on your linux command is sudo apt-get -y install git .



<bold> syntax for writing git commands is like this  $ git command options filename or directory eg. git config user.name</bold>
commands to setup git or config it one your computer manually on terminal is 1.git config --global user.name"jibrildevops"
2.git config --global user.email "jibril.os@yahoo.com"
3.to check if the configuration work you can type git config --get-all user.name or get config user.name.The terminal should 
print any username if it really worked  


##Gitcheat-codes
- git status: always run this a directory to check if the  directory has been git initialiazed. It can also be used 
to check  if the new changes have been staged and if git is tracking the new modifications 
- git init : initialiazes a git repo .git folder in its current directory
- git add . :tells git to track the new changes made to a file 
- git commit  -m "": creates a message along with the files that have been stagged and ready to be pushed to the repo
-  git restore --staged name of file : is used to unstage a file that has been staged .eg git restore --staged go.txt
- git logs : it displays all the log of committed messages as you git push the current changes.
-r m -rf  directory or folder name : deletes a directory that has been provided to it. eg rm -rf  animalfolder
- rm -f  filename :deletes a file that has been git it . 
- git log --oneline :modifies and logs and makes them more readable.
- git commit  --amend: is used to reset an already  commited message  git commit -m"" where by the default text editor is opened to the previous git commit -m"" message  .

Head: its a branch reference to its current or lastest commit on that particular branch .if say the branch you are working is 
version1 and you make a commit the  Head would point to version1 branch lastest commit.
- git branch :logs all the branches in the repo.
- git branch branchname : creates a new branch but doesnt log into that brunch yet.eg git branch edition1 would create a new branch called edition1.
- git checkout branchname: would log us into the branch which its name has been .
- git checkout -b branchname:would create a new branch with the name given.
- git switch -also does the same thing as git branch 
- git merge branchname of the branch i want to add its modification into the current branch am into. eg am in branch main and there is modifications in branch edition1 that i want in branch man and the code would be like this git switch main ,git merge edition1 
-- warning always becareful where you branching before you safe a file 
git branch -D branchname : deletes the branch name on your local machine or local repo.
## How to Delete a branch from the remote server for the terminal

