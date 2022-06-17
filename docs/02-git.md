# **Git and Github**

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

&nbsp;

## 2. Basic commands  

- initialize a local repository in the current directory.  

```git
git init
```  

&nbsp;

- clone an entire repository from a hosted location via url.

```git
git clone [url]
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

- Add all untracked files to be tracked, ready to be commited

```git
git add .
```

&nbsp;

- Used to save the current tracked files version as a register on the version history.

```git
git commit -m “commit message”
```

&nbsp;

- Used to add all untracked files and commit on the same command.

```git
git commit -am "commit message"
```

&nbsp;

- Show all commits in the current branch history.

```git
git log
```

```git
git log --oneline
```

```git
git reflog
```

&nbsp;

- Show the Diff of what is changed but not tracked in the specific file or all files changes.

```git
git diff [file name]
```

```git
git diff
```

&nbsp;

## 3. **Remote use**

- Setup the remote repository to where you will push your code.

```git
git remote add origin [remote repository url]
```

&nbsp;

- Push your branch with the committed code to a remote repository.

```git
git push -u origin [branch name].
```

&nbsp;

## 4. **Branch**

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

## 5. **Merge**

- Merge the specified branch’s history into the current one.

```git
git merge [branch name]
```