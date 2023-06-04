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
  
  # Undo Last Commit
Undo last commit without file staged condition.(Only for local/offline repository)
- ### Undo Last Commit without file staged condition.
  ```bash
  git reset --soft HEAD^
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
  
  ## Authors

  - [@rkpust](https://www.github.com/rkpust)
