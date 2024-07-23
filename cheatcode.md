```markdown

# How to master Git and Github 


Git is software that is installed locally on your computer and can be used as for version controlling all kinds of works like writing and writing codes .
Github is the remote place where one can collaborate and word on repos stored on the cloud.

-- ⚡To install git on your linux command is sudo apt-get -y install git .



- -⚡ syntax for writing git commands is like this  $ git command options filename or directory eg. git config --global user.name commands to setup git or config it on your computer manually on terminal is :

- -⚡1.git config --global user.name"jibrildevops"

- -⚡2.git config --global user.email "jibril.os@yahoo.com"

- -⚡3.To check if the configuration work you can type git config --get-all user.name or get config user.name  .The terminal should print any username if it really worked  .


##             - -⚡Gitcheat-codes- -⚡
- -⚡ git status: always run this a directory to check if the  directory has been git initialiazed. It can also be used  to check  if the new changes have been staged and if git is tracking the new modifications .

- -⚡git init : initialiazes a git repo .git folder in its current directory.

- -⚡ git add . :tells git to track the new changes made to a file .

- -⚡git commit  -m "": creates a message along with the files that have been stagged and ready to be pushed to the repo.

- -⚡git commit -a -m"message" :commits and stages all the new modification.

- -⚡git commit  --amend: is used to reset an already  commited message  git commit -m"" where by the default text editor is opened to the previous git commit -m"" message  .

- -⚡git restore --staged name of file : is used to unstage a file that has been staged .eg git restore --staged go.txt or git restore -s filename .

- -⚡ git log --oneline : it displays all the log of committed messages as you git push the current changes and also displays the head.

- -⚡rm -rf  directory or folder name : deletes a directory that has been provided to it. eg rm -rf  animalfolder.

- -⚡rm -f  filename :deletes a file that has been git it . 

- -⚡ git log --oneline :modifies and logs and makes them more readable.
- -⚡ git diff or git diff filename  :It reveals the changes that has been made to a file or document in your current working branch .You can only use this if you havent use the command git add . That is it hasnt been staged yet.
- -⚡git diff --staged : it reveals the difference between  what has been staged area and what has been staged and ready to be committed .This command can only be used when you have used git add . i like this .
- -⚡git stash or git stash save: it stashes or saves all unstaged and stagged changes for you to go to another branch and do something quickly there and come back. it helps if your are not ready to commit the changes yet.
- -⚡git stash apply: it can help by apply the changes you have made to other branches without remove the like how git stash pop remove the stashed changes.

## Head: its a branch reference to its current or lastest commit on that particular branch .if say the branch you are working is version1 and you make a commit the  Head would point to version1 branch lastest commit.

- -⚡git branch :logs all the branches in the repo.

- -⚡- git branch branchname : creates a new branch but doesnt log into that brunch yet.eg git branch edition1 would create a new branch called edition1.
- git checkout branchname: would log us into the branch which its name has been .

- -⚡ git checkout -b branchname:would create a new branch with the name given.

- -⚡git switch -also does the same thing as git branch 

- -⚡ git merge branchname of the branch i want to add its modification into the current branch am into. eg am in branch main and there is modifications in branch edition1 that i want in branch man and the code would be like this git switch main ,git merge edition1 
- -⚡ warning always becareful where you branching before you safe a file 
- -⚡git branch -D branchname : deletes the branch name on your local machine or local repo.
- -⚡git branch -d branch_name

## How TO CREATE SSH KEYPAIR ON LOCALL MACHINE OR LAPTOP

- -⚡1. we need to check if there is an existing key pair on the machine by using this command
- -⚡`ls -al ~/.ssh`.
- -⚡it would a files with extention /_id_ed25519.pub . if this command doesnt reveal any keypair then you can go ahead and create one using this code `ssh-keygen -t ed25519 -C "jibril.os@yahoo.com` .It would ask a few question like where do you want to store the keypairs and what passphrase you want. click on enter for all. After its done use this command to reveal the public key you need to put on the remote server :  ` cat ~/.ssh/id_ed25519.pub`

## How to Delete a branch from the remote server for the terminal
## How to Delete a branch from the remote server for the terminal
```markdown
- -⚡git fetch :  Before deleting a remote branch, it's a good idea to fetch the latest changes from the remote repository to ensure you have the most up-to-date information.

- -⚡git push origin --delete branch_name :  Replace origin with the name of your remote (typically origin) and branch_name with the name of the branch you want to delete. For example, if you want to delete a branch named feature-branch, you would run: git push origin --delete feature-branch

- -⚡git branch -r  :  This will show all the remote branches. The deleted branch should no longer appear in the list.



- -⚡ git branch -M branchname renames the name of that branch provided on your local repo
- -⚡
- -⚡


# HOW TO ADD A GITHUB REMOTE TO YOUR LOCAL REPO THAT YOU HAVE CREATED

## Command 1: Add a Remote Repository

```sh
- -⚡ git remote add origin git@github.com:JOSDEVOP/git_command_cheat_codes_folders.git - -⚡

- -⚡ git remote add origin: This part of the command is telling Git to add a new remote repository with the name origin. In Git, remotes are like bookmarks to other repositories, and origin is the conventional default name for the primary remote repository.- -⚡

- -⚡ git@github.com:JOSDEVOP/git_command_cheat_codes_folders.git: This is the URL of the remote repository. It uses the SSH protocol to connect to the repository on GitHub.  - -⚡

- -⚡ The URL consists of: git@github.com: The SSH protocol prefix and the host (GitHub).- -⚡

- -⚡ JOSDEVOP: The GitHub username or organization name.- -⚡

- -⚡ git_command_cheat_codes_folders.git: The repository name.- -⚡

- -⚡ This command establishes a connection between your local repository and the specified remote repository on GitHub.- -⚡

- -⚡ git branch -M main   .git branch: This is a Git command used for branch operations.
 -M: This option stands for "move" or "rename." The -M option will rename the branch and also force the rename if a branch with the target name (main in this case) already exists.
main: This is the new name for the current branch. By default, many repositories used to name the default branch master, but main has become the new standard default branch name in many projects and platforms, including GitHub.
This command renames your current branch to main, standardizing it to modern conventions.- -⚡

- -⚡ git push -u origin main

git push: This is a Git command that updates the remote repository with commits made locally.
-u: This option stands for "set upstream." It sets the default remote tracking branch for the current local branch. After using -u, you can use git push and git pull without specifying the remote and branch names explicitly.
origin: This is the name of the remote repository. It's the same name you used in the first command when you added the remote.
main: This is the name of the branch you're pushing. It corresponds to the local branch you renamed in the second command.
This command pushes your local main branch to the origin remote repository and sets origin/main as the upstream branch for your local main branch. This makes future interactions with the main branch simpler, as you won’t need to specify the remote and branch names for subsequent git push and git pull commands.

Summary
Here’s what the entire sequence does:

Adds a remote named origin pointing to your GitHub repository.
Renames the current branch to main.
Pushes the main branch to the origin remote repository and sets it as the upstream branch for easier future interactions.
This setup ensures your local repository is properly connected to the remote repository, following modern branch naming conventions and simplifying future push and pull operations.
 - -⚡
- -⚡- -⚡
- -⚡- -⚡
- -⚡- -⚡
git branch -M main



testing edition two