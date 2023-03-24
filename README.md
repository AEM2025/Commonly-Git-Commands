# Commonly-Git-Commands
Git commands cheat sheet

_A list of my commonly used Git commands_

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
| `git log --oneline -- decorate --graph --all` | View changes in a sample line and in a graphic way |
