# Commonly-Git-Commands

_A list of commonly used Git commands_

## Git Basic Overview

![image](https://user-images.githubusercontent.com/45972231/227616699-faf07340-bea4-4536-a53a-ce2d68b2db8e.png)

### Getting & Creating Repos

| Command | Description |
| ------- | ----------- |
| `git init` | Initialize a local Git repository |
| `git clone https://github.com/[username]/[repository-name].git` | Create a local copy of a remote repository. ie: https://github.com/AEM2025/Solar-System.git |

### Basic Configuration

| Command | Description |
| ------- | ----------- |
| `git config --global user.name` | Add your username that will apear in the commit history |
| `git config --global user.email` | Add your email that will apear in the commit history |
| `git config --global init.defaultBranch main` | Change your default branch name from master to main |

### Basic Snapshotting

| Command | Description |
| ------- | ----------- |
| `git add FileName.txt` | Add a file from working directory to the staging area |
| `git add .` _OR_ `git add *` | Add all new changes from working directory to the staging area |
| `git commit -m "Commit_Message"` | Add changes from staging area to the local repo |
| `git commit -am "Commit_Message"` | Add changes from working directory to the local repo in one command |
| `git rm -r FileName.txt` | Remove a file from Repo |
| `git rm -rf .git` | Remove local Repo |
| `git status` | Check status of a specific file. |
| `git status -s` | Check status of a specific file |


![git_command_lifecycle](https://user-images.githubusercontent.com/45972231/227614077-9e9b7a42-6393-437c-af6b-d71b40e6d363.png)


### Show commit history

| Command | Description |
| ------- | ----------- |
| `git log` | View commit history. Who? When? What? SHA1? |
| `git log --summary` | View changes (summary) |
| `git log --oneline` | View commit history in a sample line |
| `git log --oneline --decorate --graph --all` | View changes in a sample line and in a graphic way |


### Sharing & Updating Projects

| Command | Description |
| ------- | ----------- |
| `git push` | Push changes to remote repository. |
| `git push [remote name] [branch name]` | Push a branch to your remote repository. Example: `git push origin master` |
| `git push -u origin [branch name]` | Push changes to remote repository (and remember the branch) |
| `git push origin --delete [branch name]` | Delete a remote branch |
| `git push --tags` | Publish tags that aren't yet in the remote repository |
| `git pull` | Update local repository to the newest commit |
| `git pull origin [branch name]` | Pull changes from remote repository |
| `git remote add origin https://github.com/[username]/[repository-name].git` | Add a remote repository |
| `git remote set-url origin https://github.com/[username]/[repository-name].git` | Set a repository's origin branch to SSH |

### Tags

| Command | Description |
| ------- | ----------- |
| `git tag <tagname>` | Tag the commits (Lightweight Tag). Example: `git tag v1.0` |
| `git tag -a <tagname>` | Tag the commits (Annotated Tag). Example: `git tag -a v1.0` |
| `git tag -a <tagname> -m "[Message]"` | Tag the commits with specific message. Example: `git tag -a v2.0 -m "version two"` |
| `git tag -d <tagname>` | Delete tag |
| `git tag` | List stored tags in a repo |
| `git checkout <tagname>` | View the state of a repo at a tag |
| `git show <tagname>` | Display all info about this tag |


### Comparison

| Command | Description |
| ------- | ----------- |
| `git diff [source branch] [target branch]` | Compare differences between files |

### Branches

| Command | Description |
| ------- | ----------- |
| `git branch` | List branches (the <strong>*</strong> denotes the current branch) |
| `git branch [branch name]` | Create a new branch |
| `git checkout -b [branch name]` | Create a new branch and switch to it in one command |
| `git branch -m [old branch name] [new branch name]` | Rename a local branch |
| `git branch -a` | List all branches (local and remote) |
| `git branch -d [branch name]` | Delete a branch |
| `git push [remote repo name] --delete [branch name]` | Delete a remote branch. Ex: git push origin --delete test_branch |
| `git checkout [branch name]` | Switch to a branch |
| `git switch [branch name]` | Switch to a branch |
| `git merge [branch name]` | Merge a branch into the active branch |
| `git merge [source branch] [target branch]` | Merge a branch into a target branch |

