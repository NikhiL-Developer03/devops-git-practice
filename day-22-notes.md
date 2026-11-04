
# Day 22 – Introduction to Git: Your First Repository

## 1. What is the difference between `git add` and `git commit`?

`git add` stages changes so they are ready to be saved. `git commit` saves the staged changes as a snapshot in Git history.

Example:

```bash
git add git-commands.md
git commit -m "Update Git commands reference"
```

## 2. What does the staging area do? Why doesn't Git just commit directly?

The staging area lets me choose which changes should go into the next commit. This is useful when I have made multiple changes but want to save only some of them together.

## 3. What information does `git log` show?

`git log` displays the commit history, including commit IDs, author details, dates, and commit messages. `git log --oneline` displays a shorter version of the history.

## 4. What is the `.git/` folder and what happens if you delete it?

The `.git/` folder stores the repository's internal information, including Git objects, configuration, references, and history. Deleting it removes the local repository metadata and normally makes the project directory stop functioning as a Git repository. The working files may remain, but the local history and branch information are lost unless backed up elsewhere.

## 5. What is the difference between a working directory, staging area, and repository?

- Working directory: Where I create and edit files.
- Staging area: Where I select changes for the next commit using `git add`.
- Repository: Where Git stores committed snapshots and their history.

