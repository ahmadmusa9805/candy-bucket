# Git Command Scribe Sheet

## Setup and Configuration
- **git config**
  - Description: Set configuration values for your user name, email, and other preferences.
  - Example:
    ```bash
    git config --global user.name "Your Name"
    git config --global user.email "your.email@example.com"
    ```

- **git config -l**
  - Description: List all the current configuration settings.
  - Example:
    ```bash
    git config -l
    ```

- **git config --global user.name/user.email**
  - Description: Set the global username and email for all repositories.
  - Example:
    ```bash
    git config --global user.name "Your Name"
    git config --global user.email "your.email@example.com"
    ```

## Basic Commands
- **ls**
  - Description: List directory contents.
  - Example:
    ```bash
    ls
    ```

- **ls -a**
  - Description: List all files, including hidden files.
  - Example:
    ```bash
    ls -a
    ```

- **git init**
  - Description: Initialize a new Git repository.
  - Example:
    ```bash
    git init
    ```

- **git clone**
  - Description: Clone a repository into a new directory.
  - Example:
    ```bash
    git clone https://github.com/user/repo.git
    ```

- **git add filename**
  - Description: Add a specific file to the staging area.
  - Example:
    ```bash
    git add filename
    ```

- **git add .**
  - Description: Add all changes in the current directory to the staging area.
  - Example:
    ```bash
    git add .
    ```

- **git reset**
  - Description: Unstage a file or set of files.
  - Example:
    ```bash
    git reset filename
    ```

- **git status**
  - Description: Show the working tree status.
  - Example:
    ```bash
    git status
    ```

- **git commit -m "message"**
  - Description: Commit the staged snapshot with a message.
  - Example:
    ```bash
    git commit -m "Initial commit"
    ```

- **git log**
  - Description: Show commit logs.
  - Example:
    ```bash
    git log
    ```

- **git diff**
  - Description: Show changes between commits, commit and working tree, etc.
  - Example:
    ```bash
    git diff
    ```

- **git show**
  - Description: Show various types of objects (commits, tags, etc).
  - Example:
    ```bash
    git show commitId
    ```

## Branching and Merging
- **git checkout -b "branchName"**
  - Description: Create a new branch and switch to it.
  - Example:
    ```bash
    git checkout -b feature-branch
    ```

- **git branch**
  - Description: List all branches.
  - Example:
    ```bash
    git branch
    ```

- **git checkout "branchName"**
  - Description: Switch to the specified branch.
  - Example:
    ```bash
    git checkout main
    ```

- **git merge "branchName"**
  - Description: Merge the specified branch into the current branch.
  - Example:
    ```bash
    git merge feature-branch
    ```

- **git branch -d "branchName"**
  - Description: Delete the specified branch.
  - Example:
    ```bash
    git branch -d feature-branch
    ```

## Advanced Commands
- **vim filename**
  - Description: Open a file in Vim editor.
  - Example:
    ```bash
    vim filename
    ```

- **cat filename**
  - Description: Concatenate and display file contents.
  - Example:
    ```bash
    cat filename
    ```

- **git config --global alias.variable "command"**
  - Description: Create a global alias for a Git command.
  - Example:
    ```bash
    git config --global alias.co checkout
    ```

- **git remote**
  - Description: Manage set of tracked repositories.
  - Example:
    ```bash
    git remote
    ```

- **git remote -v**
  - Description: Show URLs of remote repositories.
  - Example:
    ```bash
    git remote -v
    ```

- **git remote add origin link**
  - Description: Add a new remote repository.
  - Example:
    ```bash
    git remote add origin https://github.com/user/repo.git
    ```

- **git remote remove origin**
  - Description: Remove a remote repository.
  - Example:
    ```bash
    git remote remove origin
    ```

- **git fetch origin main**
  - Description: Fetch changes from the remote main branch.
  - Example:
    ```bash
    git fetch origin main
    ```

- **git pull origin main**
  - Description: Fetch and merge changes from the remote main branch.
  - Example:
    ```bash
    git pull origin main
    ```

- **git rebase origin/main**
  - Description: Rebase your current branch onto the remote main branch.
  - Example:
    ```bash
    git rebase origin/main
    ```

- **git reset HEAD~1/2/3...**
  - Description: Reset the current branch to a previous commit.
  - Example:
    ```bash
    git reset HEAD~1
    ```

- **mv oldFilename newFilename**
  - Description: Rename or move a file.
  - Example:
    ```bash
    mv oldFilename newFilename
    ```

- **git reset --hard origin/featureName**
  - Description: Reset the current branch to the state of a remote branch.
  - Example:
    ```bash
    git reset --hard origin/featureName
    ```

- **git reflog**
  - Description: Show a log of changes to the local repository.
  - Example:
    ```bash
    git reflog
    ```

- **git reflog HEAD@{int}**
  - Description: Show the reflog for a specific HEAD reference.
  - Example:
    ```bash
    git reflog HEAD@{1}
    ```

- **git cherry-pick commitId**
  - Description: Apply changes from a specific commit.
  - Example:
    ```bash
    git cherry-pick commitId
    ```

- **git stash**
  - Description: Stash the changes in a dirty working directory.
  - Example:
    ```bash
    git stash
    ```

- **git stash pop**
  - Description: Apply the most recent stash and remove it from the stash list.
  - Example:
    ```bash
    git stash pop
    ```

- **git stash list**
  - Description: List all stashed changes.
  - Example:
    ```bash
    git stash list
    ```

- **git stash apply stash@{int}**
  - Description: Apply a specific stash without removing it from the stash list.
  - Example:
    ```bash
    git stash apply stash@{1}
    ```

- **git fetch origin main**
  - Description: Fetch changes from the remote main branch (duplicate, see above).
  - Example:
    ```bash
    git fetch origin main
    ```

- **git rebase --continue**
  - Description: Continue the rebase process after resolving conflicts.
  - Example:
    ```bash
    git rebase --continue
    ```

- **git reset HEAD~[int-any without bracket]**
  - Description: Reset the current branch to a specified number of commits back.
  - Example:
    ```bash
    git reset HEAD~3
    ```

- **git reset --soft HEAD~[int]**
  - Description: Soft reset the current branch to a specified number of commits back.
  - Example:
    ```bash
    git reset --soft HEAD~3
    ```

- **git reset --hard HEAD~[int]**
  - Description: Hard reset the current branch to a specified number of commits back.
  - Example:
    ```bash
    git reset --hard HEAD~3
    ```

- **git reset --hard origin/main**
  - Description: Hard reset the current branch to match the remote main branch.
  - Example:
    ```bash
    git reset --hard origin/main
    ```

- **git rebase -i HEAD~[int]**
  - Description: Interactive rebase for a specified number of commits back.
  - Example:
    ```bash
    git rebase -i HEAD~3
    ```

- **git rebase --continue**
  - Description: Continue the rebase process after resolving conflicts (duplicate, see above).
  - Example:
    ```bash
    git rebase --continue
    ```

- **git rebase main master**
  - Description: Rebase the current branch onto another branch.
  - Example:
    ```bash
    git rebase main master
    ```

## Additional Commands
- **git tag**
  - Description: List, create, or delete tags.
  - Example:
    ```bash
    git tag
    git tag -a v1.0 -m "Version 1.0"
    ```

- **git bisect**
  - Description: Use binary search to find the commit that introduced a bug.
  - Example:
    ```bash
    git bisect start
    git bisect bad
    git bisect good commitId
    ```

- **git clean**
  - Description: Remove untracked files from the working directory.
  - Example:
    ```bash
    git clean -f
    ```

- **git archive**
  - Description: Create an archive of files from a named tree.
  - Example:
    ```bash
    git archive -o archive.zip HEAD
    ```

- **git blame**
  - Description: Show what revision and author last modified each line of a file.
  - Example:
    ```bash
    git blame filename
    ```

- **git grep**
  - Description: Print lines matching a pattern.
  - Example:
    ```bash
    git grep "TODO"
    ```

- **git shortlog**
  - Description: Summarize git log output.
  - Example:
    ```bash
    git shortlog
    ```

- **git describe**
  - Description: Give an object a human-readable name based on an available ref.
  - Example:
    ```bash
    git describe --tags
    ```

- **git rm**
  - Description: Remove files from the working tree and from the index.
  - Example:
    ```bash
    git rm filename
    ```

- **git mv**
  - Description: Move or rename a file, a directory, or a symlink.
  - Example:
    ```bash
    git mv oldFilename newFilename
    ```

- **git diff --staged**
  - Description: Show changes between the index and the last commit.
  - Example:
    ```bash
    git diff --staged
    ```

This `README.md` file now includes a comprehensive list of both basic and advanced Git commands, with descriptions and examples. Ensure you review and adjust any descriptions or examples as needed to match the specifics of your course or personal preferences.
