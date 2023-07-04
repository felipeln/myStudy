# **Git and Github**

## **Summary**

[1 - Git Config](#1-config)

[2 - Git Basics commands](#2-basic-commands)

[3- Git reset commands](#3-reset-commands)

[4 - Git Remote use commands](#4-remote-use)

[5 - Git branch commands](#5-branch)

[6 - Git Merge commands ](#6-merge)

[7 - Github](#7-github)

## **What is git ?**

Git is a version control system that helps you keep the track on code changes and is used to collaborate on coding.


## 1. **Config**

- Setup the name for credit when reviewing version history.

```git
git config --global user.name “user full name”
```

&nbsp;

- Setup the email address that will be used at github to history marker.

```git
git config --global user.email “github account email”
```

- Setup the git default code editor

```git
git config --global code.editor [code editor name]
```

&nbsp;

## 2. **Basic commands**  

- Initialize a local repository in the current directory.  

```git
git init
```

&nbsp;

- Show modified files in working directory, tracked and untracked for your next commit

```git
git status
```

&nbsp;

- Add untracked files to be tracked, ready to be committed.

```git
git add “file name”
```

&nbsp;

- Add all untracked files to be tracked (staged area), ready to be commited

```git
git add .
```

&nbsp;

- Used to save the current tracked files version as a snapshot register on the version history.

```git
git commit -m “commit message”
```

&nbsp;

- Used to add all untracked files and commit them on the same command.

```git
git commit -am "commit message"
```

&nbsp;

- Used to change last commit message.
```git
git commit --amend
```

&nbsp;

- Show all commits in the current branch history with the commit hash, author name, date, time and the commit message

```git
git log
```

&nbsp;

- Show all commits in the current branch history with the commit hash in a short form.

```git
git log --oneline
```

&nbsp;

- used to show the record updates made to the tip of branches.

```git
git reflog
```

&nbsp;

- Show the Diff of what is changed but not tracked or staged in the specific file or all files changes.

```git
git diff [file name]
```

&nbsp;

- Show only the name of the files that was modified.

```git
git diff --name-only
```

&nbsp;

- Show all commits with commit hash, branch, author, date, commit message and what was modified.

```git
git show
```

&nbsp;

- Show a specified commit with commit hash, branch, author, date, commit message and what was modified.

```git
git show [commit hash]
```

&nbsp;

- go back to the last commited change of the file.

```git
git checkout [file name]
```

&nbsp;

## 3. **Reset commands**

- Remove the file from the staging area ( from ready to be commmited )

```git
git reset HEAD [file name]
```

&nbsp;

- Will remove the commit but keep the changes on the files and the files will be ready to be commited
  - **obs:** you will pass the previous commit hash, not the hash from the commit you want to delete.

```git
git reset --soft [previous commit hash]
```

&nbsp;

- Will remove the commit but keep the changes but not added to be tracked 
  - **obs:** you will pass the previous commit hash, not the hash from the commit you want to delete.

```git
git reset --mixed [previous commit hash]
```

&nbsp;

- Will remove any commit and changes ahead the commit hash passed.

```git
git reset --hard [previous commit hash]
```

## 4. **Remote use**

- Setup the remote repository to where you will push your code.

```git
git remote add origin [remote repository url]
```

&nbsp;

- Shows the current remote repository

```git
git remote -v
```

&nbsp;

- clone an entire repository from a hosted location via url, to your computer.

```git
git clone [url]
``` 

&nbsp;

- Updates the local repository with changes from the remote repository.

```git
git pull
```

&nbsp;

- Push your branch with the committed code to a remote repository.

```git
git push -u origin [branch name].
```

&nbsp;

## 5. **Branch**

- to create a new branch.

```git
git branch [branch name]
```

&nbsp;

- To create a new branch and switch to then.
  - **obs:** branch are normally used to implement new features without break the code that is already working, so create a branch for code this feature.  

```git
git checkout -b [branch name]
```

&nbsp;

- Switch to another branch.

```git
git checkout [branch name]
```

&nbsp;

- List all remotes and local branches

```git
git branch
```

&nbsp;

- List all remotes and local branches with commit logs

```git
git branch -v
```

&nbsp;

- Change the current branch name

```git
git branch -m [new branch name] 
```

&nbsp;

- Delete the branch

```git
git branch -d [branch name]
```

&nbsp;

## 6. **Merge**

- Merge the specified branch’s history into the current one.

```git
git merge [branch name]
```

## 7. **Github**

Github is service where you can store and manage your code on the cloud, with github you can have remotes repositories with your codes.

:octocat: [github](https://github.com/)