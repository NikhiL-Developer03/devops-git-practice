
# Git Commands Reference

## 1. Setup & Config

### Check Git Version
```bash
git --version
```
Shows the installed Git version.

Example: `git --version`

### Configure Username
```bash
git config --global user.name "Your Name"
```
Sets the name used for your commits.

Example: `git config --global user.name "NikhiL-Developer03"`

### Configure Email
```bash
git config --global user.email "your@email.com"
```
Sets the email used for your commits.

Example: `git config --global user.email "nikhil.developer03@gmail.com"`

### View Configuration
```bash
git config --global --list
```
Displays your global Git settings.

Example: `git config --global --list`

## 2. Basic Workflow

### Initialize a Repository
```bash
git init
```
Creates a new Git repository in the current directory.

Example: `git init`

### Check Repository Status
```bash
git status
```
Shows the current branch and the status of tracked and untracked files.

Example: `git status`

### Stage a File
```bash
git add filename
```
Stages a file so it can be included in the next commit.

Example: `git add git-commands.md`

### Commit Changes
```bash
git commit -m "Meaningful message"
```
Records the staged changes in repository history.

Example: `git commit -m "Add Git commands reference"`

## 3. Viewing Changes

### View Working Directory Changes
```bash
git diff
```
Shows unstaged changes to tracked files.

Example: `git diff`

### View Staged Changes
```bash
git diff --staged
```
Shows changes currently staged for the next commit.

Example: `git diff --staged`

### View Commit History
```bash
git log
```
Displays commit history, including commit IDs, authors, dates, and messages.

Example: `git log`

### View Compact Commit History
```bash
git log --oneline
```
Displays each commit on a single line.

Example: `git log --oneline`

## 4. File & Directory Commands

### List Files
`ls` lists files and directories in the current directory.

Example: `ls -la`

### Print Working Directory
`pwd` displays the current directory path.

Example: `pwd`

### Create a Directory
`mkdir` creates a new directory.

Example: `mkdir practice`

### Create an Empty File
`touch` creates an empty file if it does not exist.

Example: `touch notes.txt`

### Change Directory
`cd` changes the current working directory.

Example: `cd practice`

## 5. Branching Commands

### List Branches
`git branch` lists local branches.

Example: `git branch`

### Create a Branch
`git branch branch-name` creates a new branch.

Example: `git branch feature-notes`

### Switch Branch
`git switch branch-name` switches to an existing branch.

Example: `git switch master`

### Create and Switch to a Branch
`git switch -c branch-name` creates a branch and switches to it.

Example: `git switch -c feature-notes`

## 6. Useful Git Commands

### Show Commit Details
`git show` displays details and changes from a commit.

Example: `git show HEAD`

### Show the Current Branch
`git branch --show-current` displays the current branch name.

Example: `git branch --show-current`

### Check Differences Between Commits
`git diff HEAD~1 HEAD` shows changes between the latest two commits.

Example: `git diff HEAD~1 HEAD`

### Show Short Repository Status
`git status --short` displays a compact summary of file changes.

Example: `git status --short`



### Step 3.1: Understand the .git/ contents
Item	Purpose
HEAD	Identifies the branch or commit currently checked out.
config	Stores repository-specific settings.
objects/	Stores Git's internal objects and data.
refs/	Stores references to branches and tags.
hooks/	Contains sample scripts that can run during Git events.
info/	Contains additional repository information.
description	Repository description, mainly used by some Git hosting tools.
branches/	Legacy directory related to branch references.
