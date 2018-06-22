# Using Git

## Setup

- See where Git is located: which git

- Get the version of Git: git --version

- Create an alias (shortcut) for git status: git config --global alias.st status

## General Commands

- Initialize Git: git init

- Get everything ready to commit: git add .

- Get custom file ready to commit: git add index.html

- Commit changes: git commit -m "Message"

- Add and commit in one step: git commit -am "Message"

- Remove files from Git: git rm index.html

- Update all changes: git add -u

- Remove file but do not track anymore: git rm --cached index.html

- Move or rename files: git mv index.html dir/index_new.html

- Undo modifications (restore files from latest commited version): git checkout -- index.html

- Restore file from a custom commit (in current branch): git checkout 6eb715d -- index.html

## Update and delete

- Test-Delete untracked files: git clean -n

- Delete untracked files (not staging): git clean -f

- Unstage (undo adds): git reset HEAD index.html

- Update most recent commit (also update the commit message): git commit --amend -m "New Message"
