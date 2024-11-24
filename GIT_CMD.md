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

- git log
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

# Git Merge and Rebase
- Main A -> B -> C -> D ->Go Feature -> G
- Feature -  E -> F
- Merge A-> B-> C -> D ->E ->F ->G- > H (H -> one extra commit for merge)
- Rebase  A-> B-> C -> D-> G ->E ->F

# Git fetch and Pull
- Fetch -> fetch show us the notification that is there any update is available on remote if branch is up to date the nothing will show on 'git fetch' cmd ( After taking fethc need to merge the changes )
- Pull -> It will take the change and merge with it

# .gitkeep -- create track of empty flder create a file  inside that folder
git remote add [alias as origin] URL
git add filename ( add specific file )
git add . ( . means all files )
git push -u origin develop ( used to push changes on develop -u -> --set-upstream )
git checkout -b develop ( create a new branch with all checkout )
git checkout master ( change current branch to master branch )
git pull origin master ( taking lastest changes from master branch )
git status ( to checck status )
git pull ( get update in current remote branch )
git pull origin branch_name (git chnaes in local acctive branch from remove branch_name )
git stash
git stash list
git stash apply ( after apply the stash needs to remove )
git stash pop/drop
git branch ( all local branch )
git branch -a ( all local branch )
git diff ( to check the difference )
git reset --hard HEAD~1 ( Removed the git commit 1 count from git )
git commit --amend -m 'master2 commit' ( update the commit message)
git rebase -i HEAD~number-of commit ( :wq! for save :qa! for exit )
git config --global alias.<alias-name> '<git-command>' ( Make short alias )
log --oneline --graph --decorate --all ( Report view braching )
git mv old_directory/file.txt new_directory/new_file.txt (Show the status modified stage the we can commit direcly oterwise need to add file and shows the delted status as well )
A fork in Git is a private replica of another user's repository.
git commit --amend   ( To Add changes in last commit )
git cherry-pick ( The command git cherry-pick allows you to choose and apply specific commits from one branch to another. )
git cherry-pick --edit <commit>… ( for edit the commit message )
git rm file_name ( after remove file we can directly commit from modified stage if i will delete directly then need to add then commit  )

git restore --staged <file> ( It removes a specified file from the staging area, but keeps the changes in the working directory. (.dot, file, directory) )