# Git Commands Cheat Sheet

This document provides a summary of commonly used Git commands for managing your repositories.

## Configuration

Set your user name and email globally:

```
git config --global user.name "Your Name"
git config --global user.email "your_email@example.com"
```

# Initialize a Repository

```
git init
```

# Cloning a Repository

```
git clone <repository_url>
```

# Adding Files

```
git add <file_or_directory>
git add .
```

# Committing Changes

```
git commit -m "Commit message"
```

# Checking Status

```
git status
```

# Viewing Commit History

```
git log
```

# Pushing Changes

```
git push origin <branch_name>
```

# Pulling Changes

```
git pull origin <branch_name>
```

# Branching

```
git branch <new_branch_name>
git checkout <branch_name>
git checkout -b <new_branch_name>
```

# Merging

```
git merge <branch_name>
```

# Viewing Differences

```
git diff
git diff <source_branch> <target_branch>
```

# Removing Files

```
git rm <file>
```

# Resetting Changes

```
git reset --soft <commit_hash>
git reset --hard <commit_hash>
```

# Amending Commits

```
git commit --amend -m "New commit message"
```

# Working with Remotes

```
git remote add <remote_name> <remote_url>
git fetch <remote_name>
git remote -v
git remote remove <remote_name>
```

# Clone the Repository

```
git clone <repository_url>
cd <repository_name>
```

# Create a Branch for a New Feature

```
git checkout -b new-feature
```

# Make Changes and Commit

```
git add .
git commit -m "Add new feature"
```

# Push the Feature Branch

```
git push origin new-feature
git checkout main
git pull origin main
```

# Set Up SSH

```
ssh-keygen -t ed25519 -C "your_email@example.com"

```

# Renaming a Git Branch

This guide explains how to rename a Git branch both locally and remotely.

## Rename a Local Branch

1. **Switch to a Different Branch**

   - You cannot rename the branch you're currently on. Switch to a different branch (e.g., `main` or `master`):
     ```bash
     git checkout main
     ```

2. **Rename the Branch**
   - Use the `git branch -m` command to rename the branch. Replace `old-branch-name` with the current branch name and `new-branch-name` with the new name you want:
     ```bash
     git branch -m old-branch-name new-branch-name
     ```

## Rename a Remote Branch

1. **Push the Renamed Branch**

   - Push the newly named branch to the remote repository:
     ```bash
     git push origin new-branch-name
     ```

2. **Delete the Old Branch from Remote**

   - Remove the old branch name from the remote repository:
     ```bash
     git push origin --delete old-branch-name
     ```

3. **Update Your Local Repository**
   - If other team members have the old branch name, they’ll need to fetch the changes and update their references:
     ```bash
     git fetch origin
     ```

## Notes

- Make sure to inform your team about the branch rename to avoid confusion.
- Update any references to the old branch name in your project or documentation.

For further assistance, refer to the [Git documentation](https://git-scm.com/doc).
