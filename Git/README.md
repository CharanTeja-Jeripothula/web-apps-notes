# web-apps-notes

## Github commands

- git init - initializes a git repository in the current working directory
- git add <file> - adds the file mentioned into staging area.
- git add . - adds all files in the current directory to the staging area
- git status - Displays the current status of the repository, including modified, staged, and untracked files
- git commit -m "message" - commits the changes in the staging area with a message
- git pull - Fetches the latest changes from a remote repository and merges them into the current branch.
- git pull origin master - pulls the changes from the remote repository
- git push - Pushes the local commits to a remote repository, updating it with the latest changes.
- git push origin master - pushes the changes to the remote repository
- git clone https://github.com/username/repository.git - clones the repository to the local machine
- git remote add origin https://github.com/username/repository.git - adds the remote repository to the local repository
- git remote -v - displays the remote repositories
- git branch - lists the branches in the local repository
- git checkout -b <branch-name> - creates a new branch and switches to it
- git checkout <branch-name> - switches to the specified branch
- git merge <branch-name> - merges the specified branch into the current branch
- git log - displays the commit history
- git reset --hard HEAD~1 - reverts the changes to the previous commit
- git stash - saves the changes in the working directory
- git stash pop - applies the changes saved in the stash
- git diff - Shows the differences between the working directory and the staging area or the repository.
- git reset <file> - Removes a file from the staging area, preserving its changes in the working directory.
- git rm --cached <file-name> - removes the file from the tracking list without deleting it from your local file system.
- git clone -b <branch-name> <repository-url> - clone a specific branch 
- git fetch - fetches all the changes from the remote repo allowing you to view the changes without automatically merging them with the local repo.

- git push --set-upstream origin <branch-name> - if we create a branch on the local repository but it doesnt exist on the remote repository then this command will create a branch on the remote repository and push all the commits between the branches

- git push origin <branch-name> - will push the current branch to the branch of the matching name in the remote repository


# best practices

## ---This process is to be followed if we are NOT given access as a collaborator to the original repo---

- First fork the remote repository into your GITHUB account
- Clone the forked repository to your local machine
- Create a new branch for the feature you are working on
- Make changes to the files in the branch
- Commit the changes to the branch
- checkout to main branch
- fetch and merge all the latest commits from the original repo into your forked repo
- Now, pull all the changes from your forked repository into the main branch head
- merge the feature branch into the main branch in your local computer
  (solve the conflicts emerged in conflict manager of vs code and complete the commit)
- push the changes to the forked repository.
- create a pull request from your forked repository to the original repository.

## ---This process is to be followed if we are given access as a collaborator to the original repo---

- First clone the remote repository into the local computer
- Create a new branch for the feature you are working on
- Make changes to the files in the branch
- Commit the changes to the branch
- checkout to main branch
- pull all the changes from the remote repository into the main branch head
- merge the feature branch into the main branch
  (solve the conflicts emerged in conflict manager of vs code and complete the commit)
- push the changes to the remote repository.


## Solving Merge Conflicts
- Its always recommended to use merge conflict solver in Visual Studio Code
- Otherwise, search for <<<<<<,=======,>>>>>> symbols in the files which suggest the conflicting parts of code. 
- Then manually solve the conflicts.
- After solving the conflicts, add the changes to the staging area and commit the changes. (":wq" is to be used to save and exit from the merge conflict editor in vim/hyper )
- Push the changes to the remote repository.



