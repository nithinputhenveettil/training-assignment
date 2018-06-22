# Git Commands

### Tell Git who you are

Configure the author name and email address to be used with your commits.
Note that Git strips some characters (for example trailing periods) from user.name.
```
git config --global user.name "Sam Smith"
git config --global user.email sam@example.com
```

### Create a new local repository
```
git init
```

### Check out a repository

Create a working copy of a local repository:
```
git clone /path/to/repository
```
For a remote server, use:
```
git clone username@host:/path/to/repository
```

### Add files	

Add one or more files to staging (index):
```
git add <filename>

git add *
```

### Commit

Commit changes to head (but not yet to the remote repository):
```
git commit -m "Commit message"
```
Commit any files you've added with git add, and also commit any files you've changed since then:
```
git commit -a

### Push

Send changes to the master branch of your remote repository:
```
git push origin master
```

### Status

List the files you've changed and those you still need to add or commit:
```
git status
```

### Connect to a remote repository

If you haven't connected your local repository to a remote server, add the server to be able to push to it:	
```
git remote add origin <server>
```

### Branches

Create a new branch and switch to it:
```
git checkout -b <branchname>
```
Switch from one branch to another:	
```
git checkout <branchname>
```
List all the branches in your repo, and also tell you what branch you're currently in:	
```
git branch
```
Delete the feature branch:	
```
git branch -d <branchname>
```
Push the branch to your remote repository, so others can use it:	
```
git push origin <branchname>
```
Push all branches to your remote repository:	
```
git push --all origin
```
Delete a branch on your remote repository:	
```
git push origin :<branchname>
```






