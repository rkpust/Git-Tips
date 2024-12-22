# Git-Tips
Git Practices 


# User Email & Name 
- ### To Set User Email
  ```bash
  git config --global user.email "you@example.com"
  ```
- ### To Set User Name
  ```bash
  git config --global user.name "Your Name"
  ```
  
# Add File & Remove
For All File Replace FileName by .
- ### To Add File
  ```bash
  git add "FileName"
  ```
- ### To Remove File
  ```bash
  git restore --staged "FileName"
  ```

- ### Ensure venv Is Not Already Tracked by Git
  If the venv folder was already tracked by Git before adding it to .gitignore, you'll need to remove it from Git's tracking. Run the following command:
  ```bash
  git rm -r --cached venv/
  ```
  
  # Undo Last Commit
Undo last commit without file staged condition.(Only for local/offline repository)
- ### Undo Last Commit without file staged condition.
  ```bash
  git reset --soft HEAD^
  ```

# Branch Tips
- ### To Create New Branch
  ```bash
  git branch branch-name
  ```

- ### To Checkout New Branch
  ```bash
  git checkout branch-name
  ```
- ### To create a new branch and switch to it at the same time
  ```bash
  git checkout -b branch-name
  ```

- ### To delete a branch
   To delete a branch, you must leave off the branch that you want to delete and run this command.
  ```bash
  git branch --delete branch-name
  ```
  
# OS changed but user same
When our OS is changed but user and directory is same.
- ### To add an exception for this directory
  ```bash
  git config --global --add safe.directory 'Directory With Path'
  ```
then, add email and user name.
  
# To Clean/Remove Untracked/Uncommit File
 This command is recursive and cleans both the current directory and any subdirectories.
- ### To Remove File
  ```bash
  git clean -f -d
  ``` 
# To Update File From Remote Repo To Local Repo
 This command will help when remote repo has changed as well as we need to change in local repo.
- ### To change in local repo
  ```bash
  git pull
  ```
# To discard local changes to all files, permanently
 This command will help when local repo has changed as well as we not need to change in remote repo.
- ### To discard local changes
  ```bash
  git reset --hard
  ```

  # Unable to connect to github.com port 443
  When below command run,then given below error shows
  ```bash
  git push origin master
  ```
  fatal: unable to access 'https://github.com/rkpust/PostgreSQL.git/': Failed to connect to github.com port 443 after 21093 ms: Couldn't connect to server
- ### To access port
  ```bash
  git config --global http.proxy ""
  ```

  ## Authors

  - [@rkpust](https://www.github.com/rkpust)
