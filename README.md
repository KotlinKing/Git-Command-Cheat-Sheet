# Git-Command-Cheat-Sheet

When you just can't remember what a command is or don't want to use git help at the command line, this Git cheat sheet comes in handy. 😄
Since it might be challenging to learn every significant Git command by heart 💖, save this repository :bookmark: for help when you need it.

## Configuration

| Command                              | Description                                      |
| ------------------------------------ | ------------------------------------------------ |
| `git config --global user.name "Your Name"` | Set your Git username                         |
| `git config --global user.email "youremail@example.com"` | Set your Git email address              |
| `git config --global --list`         | List your Git configuration                      |
<hr>

## Repository Initialization

| Command                              | Description                                      |
| ------------------------------------ | ------------------------------------------------ |
| `git init`                           | Initialize a new Git repository                   |
| `git clone <repository-url>`         | Clone a remote repository to your local machine   |
<hr>

## Branching and Merging

| Command                              | Description                                      |
| ------------------------------------ | ------------------------------------------------ |
| `git branch`                         | List all branches                                |
| `git branch <branch-name>`           | Create a new branch                              |
| `git checkout <branch-name>`         | Switch to a different branch                      |
| `git merge <branch-name>`            | Merge changes from a branch into the current branch |
| `git push origin <branch-name>`      | Push a branch to a remote repository              |
| `git pull origin <branch-name>`      | Pull changes from a remote branch                 |
| `git branch -d <branch-name>`        | Delete a branch                                  |
| `git branch -m <new-branch-name>`    | Rename the current branch                         |
| `git branch -a`                      | List all local and remote branches                |
| `git merge --abort`                  | Abort the merge in progress                       |
| `git stash branch <new-branch-name>` | Create a new branch from a stash                  |
| `git checkout -b <new-branch-name>`  | Create a new branch and switch to it              |
<hr>

## Working with Remotes

| Command                              | Description                                      |
| ------------------------------------ | ------------------------------------------------ |
| `git remote -v`                      | List all configured remotes                      |
| `git remote add <remote-name> <repository-url>` | Add a new remote repository                |
| `git remote remove <remote-name>`    | Remove a remote repository                       |
| `git fetch <remote-name>`             | Fetch changes from a remote repository            |
| `git pull <remote-name> <branch-name>` | Pull changes from a remote repository          |
| `git push <remote-name> <branch-name>` | Push changes to a remote repository            |
| `git push --tags`                    | Push tags to a remote repository                  |
| `git remote rename <old-name> <new-name>` | Rename a remote repository                   |
<hr>

## Committing Changes

| Command                              | Description                                      |
| ------------------------------------ | ------------------------------------------------ |
| `git status`                         | Show the status of your working directory         |
| `git add <file-name>`                | Add a file to the staging area                    |
| `git add .`                          | Add all changes to the staging area               |
| `git commit -m "Commit message"`     | Commit changes with a descriptive message         |
| `git commit --amend`                 | Amend the previous commit with new changes        |
| `git commit --amend -m "New message"` | Amend the previous commit with a new message   |
| `git commit --amend --no-edit`       | Amend the previous commit without editing the message |
| `git restore --staged <file-name>`   | Unstage changes in a file                         |
| `git restore <file-name>`            | Discard changes in a file                         |
| `git restore .`                      | Discard all changes in the working directory      |
| `git rm <file-name>`                 | Remove a file from the repository and working directory |
| `git mv <old-file-name> <new-file-name>` | Rename a file                                 |
<hr>

## Inspecting and Comparing

| Command                              | Description                                      |
| ------------------------------------ | ------------------------------------------------ |
| `git log`                            | Show commit history                              |
| `git log --oneline`                  | Showcommit history in one line per commit        |
| `git log --graph`                    | Show commit history as a graph                    |
| `git log --author="Author Name"`      | Show commit history by a specific author           |
| `git log --since="2 weeks ago"`       | Show commit history since a specific date         |
| `git log -- <file-name>`              | Show commit history for a specific file           |
| `git show <commit-hash>`              | Show detailed information about a commit          |
| `git diff`                           | Show changes between the working directory and the staging area |
| `git diff --staged`                  | Show changes between the staging area and the last commit |
| `git diff <commit-hash>`             | Show changes between a specific commit and the working directory |
| `git diff <commit-hash>..<commit-hash>` | Show changes between two specific commits       |
| `git blame <file-name>`               | Show who changed each line in a file and when     |
| `git stash list`                     | List all stashes                                 |
| `git stash show`                     | Show changes in the most recent stash             |
| `git stash show -p <stash-index>`     | Show changes in a specific stash                  |
| `git stash drop`                     | Remove the most recent stash                      |
| `git stash drop <stash-index>`        | Remove a specific stash                           |
<hr>

## Working with Tags

| Command                              | Description                                      |
| ------------------------------------ | ------------------------------------------------ |
| `git tag`                            | List all tags                                    |
| `git tag <tag-name>`                 | Create a new lightweight tag                      |
| `git tag -a <tag-name> -m "Tag message"` | Create an annotated tag with a message        |
| `git tag -d <tag-name>`              | Delete a specific tag                             |
| `git push origin --tags`             | Push tags to a remote repository                  |
| `git checkout <tag-name>`            | Switch to a specific tag                          |
| `git describe <commit-hash>`         | Show the most recent tag reachable from a commit  |
<hr>

## Collaboration

| Command                              | Description                                      |
| ------------------------------------ | ------------------------------------------------ |
| `git fetch`                          | Fetch changes from the remote repository          |
| `git pull`                           | Pull changes from the remote repository           |
| `git push`                           | Push changes to the remote repository             |
| `git push -f`                        | Force-push changes to the remote repository       |
| `git push origin --delete <branch-name>` | Delete a remote branch                         |
| `git cherry-pick <commit-hash>`      | Apply the changes introduced by a specific commit |
| `git rebase <branch-name>`            | Reapply commits on top of another branch          |
| `git rebase --abort`                 | Abort a rebase in progress                        |
| `git rebase --continue`              | Continue a rebase after resolving conflicts       |
| `git rebase --skip`                  | Skip a commit during a rebase                     |
| `git remote prune origin`            | Remove remote branches that no longer exist       |
| `git blame <file-name>`               | Show who changed each line in a file and when     |
| `git shortlog`                       | Summarize git log output by author                |
| `git log --grep="<search-term>"`      | Search for commits with a specific term in the commit message |
<hr>

## Git Flow Workflow

| Command                              | Description                                      |
| ------------------------------------ | ------------------------------------------------ |
| `git flow init`                      | Initialize a Git Flow repository                  |
| `git flow feature start <feature-name>` | Start a new feature branch                      |
| `git flow feature finish <feature-name>` | Finish a feature branch                         |
| `git flow release start <release-version>` | Start a new release branch                     |
| `git flow release finish <release-version>` | Finish a release branch                        |
| `git flow hotfix start <hotfix-version>` | Start a new hotfix branch                       |
| `git flow hotfix finish <hotfix-version>` | Finish a hotfix branch                          |
| `git flow support start <support-branch>` | Start a new support branch                      |
| `git flow support finish <support-branch>` | Finish a support branch                         |
<hr>

## Rebase Workflow

| Command                              | Description                                      |
| ------------------------------------ | ------------------------------------------------ |
| `git checkout <branch-name>`         | Switch to the branch to be rebased                |
| `git rebase <base-branch>`            | Rebase the current branch onto the base branch    |
| `git rebase --continue`              | Continue after resolving conflicts during a rebase |
| `git rebase --skip`                  | Skip the current commit during a rebase           |
| `git rebase --abort`                 | Abort a rebase in progress                        |
<hr>
