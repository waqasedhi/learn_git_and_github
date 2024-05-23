
**Here's the Markdown table for the basic Git commands you provided:**

| Command | Description |
|---|:---|
| `git add <file>` | Adds a specific file to the staging area. |
| `git add .` or `git add --all` | Adds all modified and new files to the staging area. |
| `git status` | Shows the current state of your repository, including tracked and untracked files, modified files, and branch information. |
| `git commit` | Creates a new commit with the changes in the staging area and opens the default text editor for adding a commit message. |
| `git commit -m "<message>"` or `git commit --message "<message>"` | Creates a new commit with the changes in the staging area and specifies the commit message inline. |
| `git commit -am "<message>"` or `git commit --all --message "<message>"` | Commits all modified and deleted files in the repository without explicitly using `git add` to stage the changes. |
| `git reset <file>` or `git reset` | Reset file in the working directory to its unstage area. |
| `git reset <commit_id>` | Moves the branch pointer to a specified commit, resetting the staging area and the working directory to match the specified commit. |
| `git reset --hard <commit_id>` | Moves the branch pointer to a specified commit, discarding all changes in the staging area and the working directory, effectively resetting the repository to the specified commit. |
| `git rm <file>` | Removes a file from both the working directory and the repository, staging the deletion. |
| `git mv` | Moves or renames a file or directory in your Git repository. |
|`git log`|Displays the commit history of the current branch.|
|`git log –all`|Displays the commit history of all branches.|

<br><br>

**This is file life-cycle on local repo**
![](images/git-lifecycle.png)
<br><br><br><br>

**This is work-flow image on local to remote repo**
![](images/git-workflow.png)
<br><br>

**Branching and Merging**
**Here are some Git branching and merging commands:**

| Command                       | Description                                                                       |
|-------------------------------|:-----------------------------------------------------------------------------------|
| `git branch`                  | Lists all branches in the repository.                                               |
| `git branch <branch-name>`    | Creates a new branch with the specified name on current branch.                                      |
| `git branch -d <branch-name>` | Deletes the specified branch.                                                       |
| `git branch -a`               | Lists all local and remote branches.                                               |
| `git switch <branch-name>`    | Switches to the specified  branches.                                                         |
| `git checkout <branch-name>`  | Switches to the specified branch.                                                  |
| `git checkout -b <new-branch-name>` | Creates a new branch and switches to it.                                             |
| `git merge <branch>`           | Merges the specified branch into the current branch.                                 |
| `git log`                     | Displays the commit history of the current branch.                                  |
| `git log <branch-name>`       | Displays the commit history of the specified branch.                                 |
| `git log --all`               | Displays the commit history of all branches.                                       |
| `git diff` | Shows the changes between the working directory and the staging area (index). |
| `git diff <commit1> <commit2>` | Displays the differences between two commits. |

**This is how branches are managed on git**
![](images/git-tutorials-How-Git-branches-work.webp)
<br><br>

**Remote Repositories**
**Here are some Git remote repositories commands:**

| Command                 | Description                                                                                                  |
|-------------------------|:--------------------------------------------------------------------------------------------------------------|
| `git fetch`              | Retrieves changes from a remote repository, including new branches and commits.                          |
| `git pull`               | Fetches changes from the remote repository and merges them into the current branch.                         |
| `git pull <remote>`      | Fetches changes from the specified remote repository and merges them into the current branch.                |
| `git push`               | Pushes local commits to the remote repository.                                                             |
| `git push <remote>`      | Pushes local commits to the specified remote repository.                                                   |
| `git push <remote> <branch>` | Pushes local commits to the specified branch of the remote repository.                                     |
| `git push --all`         | Pushes all branches to the remote repository.                                                                |