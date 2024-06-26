# web-apps-notes

# Github commands

- git init - initializes a git repository in the current working directory
- git add . - adds all files in the current directory to the staging area
- git commit -m "message" - commits the changes in the staging area with a message
- git push origin master - pushes the changes to the remote repository
- git pull origin master - pulls the changes from the remote repository
- git clone https://github.com/username/repository.git - clones the repository to the local machine
- git remote add origin https://github.com/username/repository.git - adds the remote repository to the local repository
- git remote -v - displays the remote repositories
- git branch - lists the branches in the local repository
- git checkout -b branch-name - creates a new branch and switches to it
- git checkout branch-name - switches to the specified branch
- git merge branch-name - merges the specified branch into the current branch
- git log - displays the commit history
- git reset --hard HEAD~1 - reverts the changes to the previous commit
- git stash - saves the changes in the working directory
- git stash pop - applies the changes saved in the stash

- git push --set-upstream origin <branch-name> - if we create a branch on the local repository but it doesnt exist on the remote repository then this command will create a branch on the remote repository and push all the commits between the branches

# best practices

---This process is to be followed if we are given access as a collaborator to the original repo---

- First clone the remote repository into the local computer
- Create a new branch for the feature you are working on
- Make changes to the files in the branch
- Commit the changes to the branch
- checkout to main branch
- pull all the changes from the remote repository into the main branch head
- merge the feature branch into the main branch
  (solve the conflicts emerged in conflict manager of vs code and complete the commit)
- push the changes to the remote repository.
