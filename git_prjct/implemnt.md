# The Git Project Documentation #
### Aim: To initialise a repository locally and migratr to remote github location
+ Create a directory to initialise it 
  
![initialise Repo](/git_prjct/git_init.JPG)
+ When the  directory or path is initialised it is set to master, our next goal is to set it to main as the github always set a repo to main
+ We create and switch to a **main** branch `git checkout -b main` and 
+ Merge master to main `git merge master`
+ After the branch has been merged, delete the **master** branch
![merging branches](/git_prjct/first.JPG)
![merging branches 2](/git_prjct/2nd.JPG)
+ Its time to migrate our locally created repository  to a github remote repo by using the following commands
 #### You must always make sure your current working directory is the directory that has been git initialised
 #### Set up a new repo on github and get the git url
 #### Run ` git remote add origin https://github.com/Coffeedcognac/Test_git.git` to migrate all files from the initialised local repo to the github url
 #### To clone a repo from github ` git clone origin https://github.com/Coffeedcognac/Test_git.git` ###
  ![merging branches 2](/git_prjct/3rd.JPG)
