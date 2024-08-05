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
#Set Up SSH
```
ssh-keygen -t ed25519 -C "your_email@example.com"

```
