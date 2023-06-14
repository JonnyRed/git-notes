# GitHub Notes

A set of cheatsheet Git notes that I find useful in my usage of
Git.

## Table of Contents

- [Introduction](#introduction)
- [Content](#content)
- [Introduction to Git and GitHub](#introduction-to-git-and-github)


---

# Git Quick Notes

## Introduction

Welcome to my collection of Git quick notes! As I navigate my way through Git and its various intricacies, I often find myself forgetting certain aspects or commands. These notes serve as a compilation of the valuable bits and pieces that I come across and want to remember for future reference.

In this repository, you'll find a collection of concise and practical notes that I've gathered while working with Git. These notes aim to provide quick reminders, helpful tips, and useful snippets that can assist both beginners and experienced users in their Git journeys.


Please note that these are personal notes, so they reflect my own experiences and preferences. If you find any errors, I encourage you to open an issue or submit a pull request.


## Content

1. Git Configuration:
   - `git config --global user.name "John Reynolds"`: Sets up Git with your name.
   - `git config --global user.email "jjmreynolds@gmail.com"`: Sets up Git with your email.
   - `git config --global color.ui auto`: Makes sure that Git output is colored.
   - `git config --global merge.conflictstyle diff3`: Displays the original state in a conflict.
   - `git config --list`: Display configuration options.

2. Bash commands:
   - `ls`: Used to list files and directories.
   - `mkdir`: Used to create a new directory.
   - `cd`: Used to change directories.
   - `rm`: Used to remove files and directories.
   - `pwd`: Used to print the current directory.

3. Git commands:
   - `git init`: Initializes an empty Git repository.
   - `git clone <repository>`: Creates an identical copy of an existing repository.
   - `git remote -v`: Lists remote repositories.
   - `git log`: Shows commit history.
   - `git status`: Shows the status of the working directory.
   - `git add <files>`: Moves files from the working directory to the staging index.
   - `git commit`: Saves files from the staging index to the repository.
   - `git diff`: Shows changes between commits, branches, etc.
   - `.gitignore`: File used to specify files that Git should not track.
   - `git tag`: Creates, lists, and deletes tags.
   - `git branch`: Creates, lists, and deletes branches.
   - `git merge`: Combines branches in Git, creating a merge commit.
   - `git checkout`: Switches between branches or restores files.
   - `git commit --amend`: Changes the last commit.
   - `git restore`: Undo local changes or staged local changes.
   - `git stash`: Saves local changes for later use.
   - `git reset --hard`: Discards local changes to all files permanently.


## Introduction to Git and GitHub


[Introduction to Git and GitHub] teaches you the basics of Git, a version control system, and GitHub, a web-based hosting service for Git repositories. The course covers topics such as creating and cloning repositories, working with branches, and resolving conflicts. It also includes hands-on labs that allow you to practice what you've learned.

The course is divided into three weeks.
* Week 1, you'll learn about the basics of Git and GitHub. You'll create your first repository and clone it onto your computer. You'll also learn about branches and how to use them to track changes to your code.
* Week 2, you'll learn more about working with branches. You'll learn how to merge branches and how to resolve conflicts. You'll also learn about remote repositories and how to push and pull changes from them.
* Week 3, you'll learn about some advanced Git concepts. You'll learn about tags, which are used to mark specific points in your code history. You'll also learn about rebasing and merging, which are two ways to change the history of your code.

[Introduction to Git and GitHub]:https://www.coursera.org/learn/introduction-git-github/home/week/1
