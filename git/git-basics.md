# 1. Introduction to Git

## What is Git :-
```javascript
- Git is a version control system. 
- Git helps you keep track of code changes. 
- Git is used to collaborate on code. 
- Git and GitHub are different things. 
```


## Why Git :-
```javascript
- Over 70% of developers use Git! 
- Developers can work together from anywhere in the world. 
- Developers can see the full history of the project. 
- Developers can revert to earlier versions of a project. 
```

## Features of Git :-
```javascript
- When a file is changed, added or deleted, it is considered modified 
- You select the modified files you want to Stage 
- The Staged files are Committed, which prompts Git to store a permanent snapshot of the files 
- Git allows you to see the full history of every commit. 
- You can revert back to any previous commit. 
- Git does not store a separate copy of every file in every commit, but keeps track of changes made in each commit! 
```

## What is GitHub :-
```javascript
- Git is not the same as GitHub. 
- GitHub makes tools that use Git. 
- GitHub is the largest host of source code in the world, and has been owned by Microsoft since 2018. 
```

# 2. Setting Up Git
```javascript
- Installing Git (Linux, macOS, Windows)
- Configuring Git (username, email, editor)

1. git config --global user.name “[firstname lastname]”
set a name that is identifiable for credit when review version history

2. git config --global user.email “[valid-email]”
set an email address that will be associated with each history marker

3. git config --global --list
Displays all globally configured Git settings stored in your system.

```



# 3. Basic Git Commands

```javascript
1. git init
initialize an existing directory as a Git repository

2. git clone <repository-url>
Cloning a repository:retrieve an entire repository from a hosted location via URL

3. git status
Checking the status of the repository

4. git add <file-with-extension> -> only single file
git add . -> this will add all the changes to the staging area
add a file as it looks now to your next commit (Adding files to the staging area)


5. git reset [file]
unstage a file while retaining the changes in working directory

6. git commit -m “[descriptive message]”
commit your staged content as a new commit with a message
```


## 4. Branching Basics
```javascript
1. git branch
Lists all local branches in the repository.

2. git branch -r	
Lists all remote branches.

3. git branch <branch-name>
Creates a new branch with the given name.

4. git checkout <branch-name>	
Switches to the specified branch.

5. git checkout -b <branch-name>	
Creates a new branch and switches to it immediately.

6. git checkout <branch-name>	
Switches to the specified branch.
 
7. git branch -d <branch-name>	
Deletes the specified branch if it has been merged.

8. git branch -D <branch-name>	
Force deletes the specified branch, even if it hasn’t been merged.
```



## 5. Undoing Changes
```javascript
> Undo Unstaged Changes (Working Directory)


1. git checkout -- <file>	
Discards changes in a specific file (before staging).

2. git restore <file>	
Alternative to checkout (recommended in newer Git versions).

3. git restore .	
Discards all unstaged changes in the working directory.
```



```javascript
> Undo Staged Changes (Before Commit)

1. git reset <file>	
Unstages a specific file (keeps changes in working directory).

2. git reset	
Unstages all staged files.

3. git restore --staged <file>	
Another way to unstage a specific file.
```

```javascript
> Undo a Commit (Before Pushing)

1. git reset --soft <commit>	
Moves to the specified commit but keeps changes staged (ready for commit).

2. git reset --mixed <commit> (default)	
Moves to the specified commit, unstages changes, but keeps them in the working directory.

3. git reset --hard <commit>
Moves to the specified commit and removes all changes (both staged and in the working directory).
```


```javascript
> Undo a Commit (After Pushing)

1. git revert <commit-hash>
Creates a new commit that undoes a specific commit (safe for shared branches).

2. git reset --hard <commit-hash>	
Resets to a specific commit, removing all changes after it (not recommended if already pushed).

3. git push --force	
Forces changes to the remote repository (use with caution).
```

```javascript
>  Undo Changes with Stash
// Git stash is used to temporarily save changes without committing them, allowing you to switch branches or work on something else without losing progress.

> Save Uncommitted Changes

1. git stash
Stashes all modified and staged changes.

2. git stash -u	
Stashes all changes, including untracked files.

3. git stash push -m "message"	
Stashes changes with a custom message for easier identification.


> View Stashed Changes

1. git stash list
Shows a list of all stashed changes.

2. git stash show
Displays a summary of the latest stash.

3. git stash show -p
Shows detailed changes of the latest stash.


> Apply or Restore Stashed Changes

1. git stash pop
Applies the latest stash and removes it from the stash list.

2. git stash apply
Applies the latest stash but keeps it in the stash list.

3. git stash apply stash@{n}
Applies a specific stash from the list (e.g., stash@{1}).



> Delete Stashed Changes

1. git stash drop
Removes the latest stash.

2. git stash drop stash@{n}	
Removes a specific stash.

3. git stash clear
Deletes all stashed changes.

```