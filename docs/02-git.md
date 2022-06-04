# **Git and Github**

## 1. **Config**

- Setup the name for credit when reviewing version history.

```git
git config --global user.name “user full name”
```

- Set the email address that will be used at github to history marker.

```git
git config --global user.email “github account email”
```

## 2. Basic commands

- initialize a local repository in the current directory.

```git
git init
```

- clone an entire repository from a hosted location via url.

```git
git clone [url]
``` 

- Show modified files in working directory, tracked and untracked for your next commit

```git
git status
```

- Add untracked files to be tracked, ready to be committed.

```git
git add “file name”
```

- Add all files to be tracked

```git
git add .
```

- Used to save the current tracked files version as a register on the version history.

```git
git commit -m “commit message”
```

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

- Diff of what is changed but not tracked in the specific file or all files changes.

```git
git diff [file name]
```

```git
git diff
```

## 3. **Remote use**

- Setup the remote repository to where you will push your code.

```git
git remote add origin [remote repository url]
```

- Push your branch with the committed code to a remote repository.

```git
git push -u origin [branch name].
```

## 4. **Branch and merge**

- to create a new branch.

```git
git branch [branch name]
```

- To create a new branch and switch to then.
  - branch are normally used to implement new features without break the code that is already working, so create a branch for code this feature.  

```git
git checkout -b [branch name]
```

- change the current branch name

```git
git branch -m [new branch name] 
```

- switch to another branch.

```git
git checkout [branch name]
```

- merge the specified branch’s history into the current one.

```git
git merge [branch name]
```