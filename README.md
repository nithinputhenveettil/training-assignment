# Git Assignment

This assignment aims to get familiarized with basic git commands.

## Basic Git commands

This guide will give an idea about basic Git commands.

### Prerequisites

You should have Git installed in your system using

```
sudo apt-get update
sudo apt-get install git
```

## Commands

The basic Git commands includes : 

### Git init

Initializes a directory as a Git repository locally.

```
git init
```

### Git clone

It creates a working copy of a local repository

```
git clone /path/to/repository
```

For a remote server, use:

```
git clone username@host:/path/to/repository
```

### Git add

It adds one or more files to staging.
* Must run prior to a commit

```
git add <filename>
```

To add all files, use:

```
git add .
```

### Git commit

Commit changes to head (but not yet to the remote repository)

```
git commit -m "First Commit"
```

## Authors

* **Sanjo Joy** - *sanjo@qburst.com* -

## Acknowledgments

* Hat tip to anyone whose code was used
* Inspiration
* etc

