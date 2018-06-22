## GIT ASSIGNMENT

#### Submitted to NIthin Puthanveettil

### *BASIC _git_ COMMANDS*

- git init
```

This command turns a directory into an empty Git repository. This is the first step in creating a repository. After running git init, adding and committing files/directories is possible.

Usage:
``
 change directory to codebase
$ cd /file/path/to/code

 make directory a git repository
$ git init
```
In Practice:
```
 change directory to codebase
$ cd /Users/computer-name/Documents/website

 make directory a git repository
$ git init
Initialized empty Git repository in /Users/computer-name/Documents/website/.git/
```
```

-git add
```
Adds files in the to the staging area for Git. Before a file is available to commit to a repository, the file needs to be added to the Git index (staging area). There are a few different ways to use git add, by adding entire directories, specific files, or all unstaged files.

Usage:
```
$ git add <file or directory name>
```
In Practice:
```
 To add all files not staged:
$ git add .

 To stage a specific file:
$ git add index.html

 To stage an entire directory:
$ git add css
```
```

git commit
```
Record the changes made to the files to a local repository. For easy reference, each commit has a unique ID.

It’s best practice to include a message with each commit explaining the changes made in a commit. Adding a commit message helps to find a particular change or understanding the changes.

Usage:
```
 Adding a commit with message
$ git commit -m "Commit message in quotes"
```
In Practice:
```
$ git commit -m "My first commit message"
[SecretTesting 0254c3d] My first commit message
1 file changed, 0 insertions(+), 0 deletions(-)
create mode 100644 homepage/index.html
```
```
git status
```
This command returns the current state of the repository.

git status will return the current working branch. If a file is in the staging area, but not committed, it shows with git status. Or, if there are no changes it’ll return nothing to commit, working directory clean.

Usage:
```
$ git status
```
In Practice:
```
 Message when files have not been staged (git add)
$ git status
On branch SecretTesting
Untracked files:
  (use "git add <file>..." to include in what will be committed)

  	homepage/index.html

 Message when files have been not been committed (git commit)
$ git status
On branch SecretTesting
Your branch is up-to-date with 'origin/SecretTesting'.
Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

        new file:   homepage/index.html

 Message when all files have been staged and committed 
$ git status
On branch SecretTesting
nothing to commit, working directory clean
```
```

git config
```
With Git, there are many configurations and settings possible. git config is how to assign these settings. Two important settings are user user.name and user.email. These values set what email address and name commits will be from on a local computer. With git config, a --global flag is used to write the settings to all repositories on a computer. Without a --global flag settings will only apply to the current repository that you are currently in.

There are many other variables available to edit in git config. From editing color outputs to changing the behavior of git status. Learn about git config settings in the official Git documentation.

Usage:
```
$ git config <setting> <command>
```
In Practice:
```
 Running git config globally
$ git config --global user.email "my@emailaddress.com"
$ git config --global user.name "Brian Kerr"

 Running git config on the current repository settings
$ git config user.email "my@emailaddress.com"
$ git config user.name "Brian Kerr"
```
```

git branch
```
To determine what branch the local repository is on, add a new branch, or delete a branch.

Usage:
```
 Create a new branch
$ git branch <branch_name>

 List all remote or local branches
$ git branch -a

 Delete a branch
$ git branch -d <branch_name>
```
In Practice:
```
 Create a new branch
$ git branch new_feature

 List branches
$ git branch -a
* SecretTesting
  new_feature
  remotes/origin/stable
  remotes/origin/staging
  remotes/origin/master -> origin/SecretTesting
  
 Delete a branch
$ git branch -d new_feature
Deleted branch new_feature (was 0254c3d).
```
```

git checkout
```
To start working in a different branch, use git checkout to switch branches.

Usage:
```
 Checkout an existing branch
$ git checkout <branch_name>

 Checkout and create a new branch with that name
$ git checkout -b <new_branch>
```
In Practice:
```
 Switching to branch 'new_feature'
$ git checkout new_feature
Switched to branch 'new_feature'

 Creating and switching to branch 'staging'
$ git checkout -b staging
Switched to a new branch 'staging'
```
```

More commands are explained in [Reference Link](https://help.github.com/articles/basic-writing-and-formatting-syntax/)


