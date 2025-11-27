# Developer Commands Cheat Sheet

A simple reference for commonly used Git commands.

---

## Git Commands

```bash
# Delete a Local Branch
# -d it won’t delete if it has unmerged changes
# -D If you’re sure you want to delete it even if not merged
git branch -D branch_name

# Delete a Remote Branch
git push origin --delete branch_name

# Create a new branch and switch to it
git checkout -b branch_name
git switch -c branch_name

# Working changes are now saved in the stash
git stash

# Deletes the most recent stash
git stash drop

# Clear all stashes
git stash clear

# Add all files to staging area
git add . 

# Undo all files changes
git restore . 

# Add specific file to staging area
git add src/App.tsx 

# Remove all files from staging area
git restore --staged .

# Commit changes with a message
git commit -m "Add new feature"

# Bring back the files again to staging area if locally commit
# When using in push origin go back 1 commit behind in origin while the files commits are in staging
git reset --soft HEAD~1

# When using in push origin go back 1 commit behind in origin the files will not be in staging
git reset --hard HEAD~1

# Set your branch to latest updated commit only use when do (git reset --hard/soft)
git reset --soft ORIG_HEAD

# Check untracked files to remove before deleting them
git clean -n

# Check untracked files to remove before deleting them
git clean -f # remove all untracked files
git clean -f test.html # remove specific untracked files

```
