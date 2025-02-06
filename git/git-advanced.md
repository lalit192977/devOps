### Merging Branches
```javascript
1. git merge <branch-name>	
Merges the specified branch into the current branch.

2. git merge --no-ff <branch-name>
Merges with a merge commit, avoiding fast-forward.

3. git merge --squash <branch-name>	
Squashes all commits into a single commit before merging.

```

### Rebasing (Alternative to Merge)

```javascript
/*Rebasing is an alternative to merging that helps maintain
a cleaner commit history by moving or reapplying commits
from one branch to another. It avoids the extra merge
commits that clutter the history when using git merge.
*/


1. git rebase <branch>
Moves commits on top of <branch>.

2. git rebase -i HEAD~<n>
Interactive rebase for modifying commits.

3. git rebase --abort
Cancels a rebase.
```


### Working with Remote Branches
```javascript
1. git fetch origin <branch-name>
Fetches updates from a remote branch without merging.

2. git pull origin <branch-name>
Fetches and merges changes from a remote branch.

3. git push origin <branch-name>
Pushes a local branch to the remote repository.

4. git push --set-upstream origin <branch-name>	
Links a local branch to a remote branch.
```


### Deleting and Cleaning Up Branches
```javascript
1. git remote prune origin	
Deletes remote-tracking branches that no longer exist.

2. git branch --contains <commit-hash>
Shows branches that contain a specific commit.

3. git reflog	
Shows a history of all changes, including deleted branches.
```