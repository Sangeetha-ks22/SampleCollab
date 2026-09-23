 # Sync Local Changes to a GitHub Repository

This guide shows how to commit local changes and synchronize them with a GitHub repository.

## Prerequisites

- Git installed
- A GitHub repository
- The repository cloned locally

## Sync changes

```bash
# Open the repository directory
cd path/to/your-repository

# Check the current branch and changed files
git status

# Get the latest changes from GitHub
git pull origin main

# Stage all changes
git add .

# Create a commit
git commit -m "Describe the changes"

# Upload the commit to GitHub
git push origin main
```

Replace `main` with your branch name when necessary.

## Common commands

```bash
# List branches
git branch

# Switch to a branch
git switch feature/my-change

# View commit history
git log --oneline

# See unstaged changes
git diff
```

## First-time setup

```bash
git config --global user.name "Your Name"
git config --global user.email "you@example.com"
git clone https://github.com/USERNAME/REPOSITORY.git
```

## Recommended workflow

1. Run `git pull` before starting work.
2. Make and test your changes.
3. Run `git status` to review the files.
4. Stage and commit the changes.
5. Run `git push` to sync with GitHub.
