# GIT COMMANDS 

## General

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

