<h1>How to master Git and Github </h1>

<p>
.Git is software that is installed locally on your computer and can be used as for version controlling all kinds of works like writing and writing codes .
Github is the remote place where one can collaborate and word on repos stored on the cloud.
to install git on your linux command is sudo apt-get -y install git .
<bold> syntax for writing git commands is like this  $ git command options filename or directory eg. git config user.name</bold>
commands to setup git or config it one your computer manually on terminal is 1.git config --global user.name"jibrildevops"
2.git config --global user.email "jibril.os@yahoo.com"
3.to check if the configuration work you can type git config --get-all user.name or get config user.name.The terminal should 
print any username if it really worked  
</p>
##Gitcheat-codes
-git status: always run this a directory to check if the  directory has been git initialiazed. It can also be used 
to check  if the new changes have been staged and if git is tracking the new modifications 
-git init : initialiazes a git repo .git folder in its current directory
-git add . :tells git to track the new changes made to a file 
-git commit  -m "": creates a message along with the files that have been stagged and ready to be pushed to the repo
- git restore --staged name of file : is used to unstage a file that has been staged .eg git restore --staged go.txt
-git logs : it displays all the log of committed messages as you git push the current changes.
-rm -rf  directory or folder name : deletes a directory that has been provided to it. eg rm -rf  animalfolder
-rm -f  filename :deletes a file that has been git it . 
-git log --oneline :modifies and logs and makes them more readable.
<p></p>
