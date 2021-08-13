**Useful GIT Commands**  

To make any folder into git repository  
>git init
 
To configure details     
>git config --global user.name  Padma Naresh  
>git config --global user.email padmanaresh1986@gmail.com  
>git config --list  
 
To see current status of changes in git   
>git status
 
To add ciles to staging area   
>git add filename   
>git add .    
 
To commit changes to local repository  
>git commit -m "initial commit"  
 
To see commit info and Commit Hash related details   
>git log  
 
To see changes in GUI like commits and logs  
>gitk  
 

Master Branch - golden copy of production code  
Release Branch - All changes to current release will go here  
Develop Branch - Developer to deply in dev environment  
Feature Branch - To commit all features  
 
To list all branches in local  
>git branch -l  
 
To list all branches local and remote  
>git branch -a  
 
To Create Branch named develop  
>git branch develop  
 
To Switch to newly created branch   
>git switch develop  
 
To create a branch named release and switch immediately  
>git checkout -b release   
 
To create file and commit to develop branch  
>touch abc.txt  
>touch bcd.txt  
>git add .  
>git commit -m "added 2 files"  
 
To switch to master branch   
>git checkout master  
 
To merge develop branch changes to master banch    
To merge changes with history use git merge   
To merge changes with out history use git rebase   
 
>git merge develop  
>git rebase develop  

To get the latest changes from remote repository and commit in local repository  
>git pull  
 
To get the latest changes from remote repository and not commit in local repository  
developer has to decide which files need to commit in local repo  
>git fetch  
 
To puch all local changes to remote repository and commit  
>git push origin master  
 
To see all remote branches / origins  
>git remote -v  
 
To pull changes from release to master branch  
switch to master branch and run below command  
>git pull . release  
 
To clone any remote repository to local copy  
>git clone remote repo  
 
Cherry Pick is process of getting one commit rom another branch to local branch  
>git cherry-pick commit hash    
 
To Revert commits to previous state    
>git reset commit hash  
>git reset --hard commit hash  
>git reset --hard HEAD^^  (number of carrot signs represt number of steps backwords)  
 
To Stash changes in local files which is un committed work  
>git stash    
>git stash list    
>git stash pop stashid    
>git stash drop stashid  
 
To tag source code with any tag     
>git tag -a "v1.0" -m "my first tag"  
>git log  
>git tag  
>git show  
 
To see the difference between two branches    
>git diff develop...master   