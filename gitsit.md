title: How Git Works.
author: Adam Schwartz
date: 2014-01-14 18:06:07

# A Mostly Correct and Surprisingly Accurate Introduction To Git.

## Credits

### Git for Ages 4 And Up

Taught by Michael Schwern.

### Linus Torvalds

Creator of Linux and Git

## Git

### What is it

-   **Distributed** Source Code / Version Control Management System.

-   Git is not a backup solution.

### Why learn it

Besides being "fun", Git is becoming a necessary skill.

Anyone who is interested in GitHub, or ever working on a collaborative project
will benefit from knowing how Git works.

## Brief Introduction

### Common Commands

#### Do Work

-   Init

-   Clone

-   Status

-   Log

-   Add

-   Commit

#### Experimentation

-   Branch

-   Checkout

-   Merge

#### Collaboration

-   Pull

-   Push

## Init

`git init`

Creates a new Git repository in the current directory inside `.git`

## Clone

`git clone url/or/path/to/git/repository`

Copy a git repository from anywhere into a directory.

## Status

`git status`

Lists what branch you have checked out, and other helpful information about your files / the staging area. 

## Log

`git log --decorate --graph`

Prints out your commit history and displays an ASCII graph of the repository.

## Diff

`git diff file1 file2`

Useful for managing conflicts with multiple files.

## Add

`git add file`

Add is the way you write a file to Git. When you add a file, you are adding it to the staging area.

### Staging Area / The Index

The staging area is where files "wait" until you make a commit.
It is a very fundamental and important concept in Git.

## Commit

-   Every ID is unique (If the ID is the same, then all the 
    previous content is also the same)

-   Every commit is unique

### Commit Object

#### SHA Hash (ID)

-   Content

-   Author

-   Date

-   Log

-   Previous Commit

### Reference

#### Head

The `HEAD` is a reference to where you are currently working in the repository.

#### Branch

A `branch` is a "separate" part of your repository typically used to work on something (to add in later) without disturbing your previous work.

#### Tag

Similar to a branch except it marks a certain point in your commit history that will not change.
For Example: (v0.9, v1.6, v2.0)

## Branch

`git branch branchname`

Branches let you make changes to your files without "damaging" what you already have.
In other words, branching is for when you want to modify or add to your project without messing with what you are currently working on.

### Master

Master is the name of the "main" branch in your repository.

### Feature

Feature is an example branch name. In this branch we will add a *feature* to our project and then `merge` it back into `master`

## Checkout

`git checkout branchname` or `git checkout -b branchname`

Checkout is the way you switch to another branch to work on.
In the first command, you switch to a branch you have already created, and in the second example command,
you crate a branch then switch to it.

## Tagging

-   lightweight tag

`git tag tagname`

This creates a reference to the current (where the `HEAD` is) position in the repository that will **not** change.

-   annotated tag

`git tag -a tagname`

An annotated tag will be stored as a full object in the Git database and will contain similar information as a commit.
Annotated tags can also be signed and verified with GPG.

## Merge

## Rebase

## Remote

-   origin

### Fetch

### Pull

### Push

## Resources

### Reference / Tutorials

-   [Pro Git (Best)](http://git-scm.com/book)

-   [Try Git](http://try.github.io/levels/1/challenges/1)

-   [Git Simplified](http://gitolite.com/gcs.html#(3))

### Talks

-   [Git for Ages 4 And Up](https://www.youtube.com/watch?v=1ffBJ4sVUb4)

-   [Linus Torvalds on Git](https://www.youtube.com/watch?v=4XpnKHJAok8)

### Git GUI Clients

#### OS X

-   [Git-Cola](http://git-cola.github.io/)

-   [Git X](http://gitx.laullon.com/)

-   [GitHub for Mac](http://mac.github.com/)

-   Git K (Included with Git)

#### Linux

-   [Git-Cola](http://git-cola.github.io/)

-   Git K (Included with Git)

#### Windows

-   [Git-Cola](http://git-cola.github.io/)

-   [GitHub for Windows](http://windows.github.com/)

-   Git K (Included with Git)
