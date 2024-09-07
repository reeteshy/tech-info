## GIT HUM USED COMMAND (https://static.javatpoint.com/tutorial/git/download/Git%20Cheat%20Sheet.pdf)

# Get git config info

 - git config --list
 - git config --global --list
 - git config --local --list

 # Set Configuration 
 - git config --global user.name “[firstname lastname]”
 - git config --global user.email “[valid-email]”

# SETUP & INIT
- git init
- git clone

# Add Origin
- git remote add origin [branch-name]

# STAGE & SNAPSHOT
- git status
- git add
- git commit -m “[descriptive message]”
##### unstage a file while retaining the changes in working directory
- git reset 

# Git log and diff

- git log --oneline
- git diff
- git diff --staged


# TEMPORARY COMMITS
####  Save modified and staged changes
- git stash 
####  list stack-order of stashed file changes
- git stash list
####  write working from top of stash stack
- git stash pop
####  discard the changes from top of stash stack
- git stash drop
#### Saving stashes with a message
- git stash save "<Stashing Message>"
#### Check the stored stashes
- $ git stash apply
#### Stash work on a separate branch
- $ git stash branch [branch name]

# BRANCH & MERGE
####  list your branches. a * will appear next to the currently active branch
- git branch
####  create a new branch at the current commit
- git branch [branch-name]
####  switch to another branch and check it out into your working directory
- git checkout
####  merge the specified branch’s history into the current one
- git merge [branch]
#### This command will create a branch locally. To push the new branch into the remote repository
- git push -u <remote> <branch-name>

# Share and Update 
#### add a git URL as an alias
- git remote add [alias] [url]
#### fetch down all the branches from that Git remote
- git fetch [alias]
#### merge a remote branch into your current branch to bring it up to date
- git merge [alias]/[branch]
#### Transmit local branch commits to the remote repository branch
- git push [alias] [branch]
#### fetch and merge any commits from the tracking remote branch
- git pull
#### Rename the current branch name 
- git branch -m old-name new-name
#### Update the commit message
- git commit --amend -m "an updated commit message"

# Deleting Branch
- git branch -d [branch-name]