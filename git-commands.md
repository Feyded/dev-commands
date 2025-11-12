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

```
