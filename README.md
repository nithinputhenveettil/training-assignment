# Setting Global Username/Email
git config --global user.name "Aayush Tuladhar"'
git config --global user.email "aayush.tuladhar@gmail.com"'

# Clone a Repo from URL
git clone <url>

# Creating an empty GIT repository
git init

# Adding all files to Git
git add .

# Adds files to Git
git add <file1> <file2>

# Add folder to Git
git add <foldername>

# Remmove File from the Project
git rm <file1> <file2>

# Performing Commit with Message
git commit <file> -m "Message"

# Perform Commit to All Tracked Files
git commit -a -m "Message"

# Reverts changed you performed in the <filename>
git checkout -- <filename>

# All Git Commits (Reverse Chronological Order)
git log

# All Git Commits with Diffs
git log -p

# Git Log with Graph
git log --all --decorate --oneline --graph

# Show files added to the index, files with changes, and untracked files
git status

# Show unstaged changes made since your last commit
git diff

# Show changes staged for commit (i.e., difference between index and last commit)
git diff --cached

# Show changes since last commit
git diff HEAD

# Fetches from the remote and merge to the current branch
git pull

# Sync Master from Origin to Local 
git pull --rebase origin master

# Update the remote repository
git push <remote-name> <branch-name>
git push origin master

# Creates a new branch from the old branch
git checkout -b <newbranch> <oldbranch>

# Switch to <dbranch>
git checkout <branch>
git checkout -b      # -b Causes new branch to be created
git checkout -f      # -f Forcing to change branch. This is used to throw local changes

# Merge contents of <newbranch> to <oldbranch>
# The --no-ff cause merge to always create a new commit object, even if the merge should be performed with a fast-forward.

git merge --no-ff <newbranch>
git push origin develop

git checkout -b release-1.2 develop

git commit -a -m "Release Version"

git checkout master
git merge --no-ff release-1.2
git tag -a 1.2

git checkout develop
git merge --no

-ff release-1.2

git branch -d release1.2
