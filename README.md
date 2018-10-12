# Documentation
In this repository I'll contribute all my documentation and I start with Git_documentation

Git is version control system and used to keep track of changes in any set of files. It’s primarily used for source code management. It’s unique features are Committing new  changes, branching, merging and comparing all past versions. 

**Prerequisite to use Git:**   
1. Create account in Github/Bitbucket.  
2. Install git bash for your machine Linux/windows

                               Some commonly commands which use in git:    
1. git init: create a new git repository.  
2. git clone: clone git repository to your local machine.   
3. git status: display the state of the working directory and the staged snapshot.   
4. git add . : to add all the files   
5. git commit -m “some msg” : to commit all the changes from local to remote repository.  
6. git remote add origin master <server>: add project to server.  
7. git push -u origin master: push all changes to Github/Bitbucket server.  
8. git pull : pull all changes from repository to local.   
9. git branch ‘branch-name’: create new branch   
10. git checkout branch-name: pointer starts to point branch-name branch and leave master branch.   
11. git checkout -b branch-name: create new branch and switch to it in one step.   
12. git checkout merge: before merging any branch to master branch first enter into master branch  
13. git merge branch-name: merge branch with master branch and now pointer points to master branch  
14. git branch -d branch-name: delete branch  
15. git log: display history, like all commits and who did the commits.   
16. git diff: changes b/w two branches or changes b/w files in local.   
17. git fetch origin master: fetch latest history from the server  
18. git reset --hard origin/master: undo recent commit from local.   
19. git stash: save code on a stack for temporary so that user can safely switch the branch and move back to it and commit it’s code.   
20. git stash pop: remove changes from stack and place the temporary code in working directory.    
21. git stash list: display list of stash file  
22. git rm filename: remove file from repository and local both.  
23. git rm --cached filename: remove file from repository, not from local.     
  
                          There are some scenarios which we generally observe in github
                          
 **Scenario-1 : Create a new git repository in git ui and push your first project to github from      
local.**     

	Following are the steps for this scenario.      	
- create a repository with same name as of your project and don’t initialize that repository with README to avoid confusion and press OK.Use these commands to push your project:   
- cd to you project directory  
- git init    
- git add .   
- git commit -m “<any message>”  
- git remote add <git_repo_url>  
- git push -u origin master  
- Click refresh button in git ui and your project has been finally push to git ui.  
  
**Scenario-2: Create a new repository in git ui and clone to your laptop.** 

	Following are the steps for this scenario.  		
- create a repository with ReadMe file.
- git clone <git_repo_url>
- Now go on and create your project files in this directory 
- Then git commit and push to github.

**Scenario-3: Working with Project which is already present at git ui**

	Following are the steps for this scenario. 
- git clone <git_repo_url>
- Import that project into eclipse

**Scenario-4: create a development branch so that master branch will not affect from any changes** 

  Following are the steps for this scenario.  
- git branch (show only master branch)
- git checkout -b <branch_name>
- git branch (this time git branch shows two branches one is master and another created by user).
- Now make a change in your code
- git commit  -m “<commit to user-branch> ”
- git push (this will result in error that no upstream found with this branch name) 
- git push --set-upstream origin <branch_name>
- Git status  
  
**Scenario-4: Make a simple change in your project using git ui. Now pull this changes to your local and observe the result. (Import others changes into your project when your project have no changes )**

  Following are the steps for this scenario.   	
- Make a change in readme in git ui and save that 
- As git init is already initialized so no need to use it again
- git pull
- Refresh your project in eclipse and observe the result
- Eclipse will reflect changes in your code that you have added by git ui.  

**Scenario-5 Make a change in project using git ui and also make small change in your local in different line and committing both changes now pull repo changes in your local and observe the auto merge done by git. (Import others changes into your project when their change and ur change is not in same line)** 

	Following are the steps for this scenario.  
- Make a change in github ui 
- Make a change in separate file in ur local 
- git pull
- Once you hit git pull eclipse will show you both changes(git ui and local change) in your code because of auto merge
- git push
- Finally git ui also display both changes.  	

**Scenario-6  Make a small change in project using github ui and make a small change in local in same line and commit both changes and face your first merge conflicts. Now resolve this conflicts by overwriting repo changes with your local changes. (Import others changes into your project conflicting changes)**

  Following are the steps for this scenario.   
- Make a change in github ui 
- Make a change in same file/same line in ur local 
- git pull
- Now conflicts will occur and you will observe >>>>> Head and ======= symbols. Here Head represent the change that you did in local and break line represent changes of git ui. To resolve conflict remove these symbol and delete git ui changes and keep  local changes as per requirement. 
 - git push
- Local changes will be reflected at git ui.   
		
**Scenario-7 - Make a small change in project using github ui and make a small change in local in same line and commit both changes and face your first merge conflicts. Now resolve this conflicts by discarding your local change and accept repo changes**
 
  Following are the steps for this scenario.   
- Make a change in github ui 
- Make a change in same file/same line in ur local 
- git pull
- Now conflicts will occur and. This time remove local changes and keep git ui changes to resolve conflict 
- git push
- git ui changes will be reflected at git ui. 


                       


