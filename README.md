# GitHub Notes

A set of cheat sheet Git notes that I find useful in my usage of
Git.

## Table of Contents

- [Introduction](#introduction)
- [Content](#content)
- [Introduction to Git and GitHub](#introduction-to-git-and-github)
- [Git Code with Mosh][]


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


[Introduction to Git and GitHub][] teaches you the basics of Git, a version control system, and GitHub, a web-based hosting service for Git repositories. The course covers topics such as creating and cloning repositories, working with branches, and resolving conflicts. It also includes hands-on labs that allow you to practice what you've learned.

The course is divided into three weeks.
* Week 1, you'll learn about the basics of Git and GitHub. You'll create your first repository and clone it onto your computer. You'll also learn about branches and how to use them to track changes to your code.
* Week 2, you'll learn more about working with branches. You'll learn how to merge branches and how to resolve conflicts. You'll also learn about remote repositories and how to push and pull changes from them.
* Week 3, you'll learn about some advanced Git concepts. You'll learn about tags, which are used to mark specific points in your code history. You'll also learn about rebasing and merging, which are two ways to change the history of your code.

[Introduction to Git and GitHub]:https://www.coursera.org/learn/introduction-git-github/home/week/1

# The Ultimate Git Course

Welcome to **The Ultimate Git Course**! This comprehensive course will take you from a beginner to a proficient user of Git, the industry-standard version control system. Whether you're a developer, designer, or any other professional working with code or files, mastering Git is essential for efficient collaboration and project management.

## Course Overview

This course is designed to provide a hands-on learning experience, with practical examples and exercises to reinforce your understanding. You'll be guided by our experienced instructor, Mosh Hamedani, who has a passion for teaching and a wealth of expertise in software development.

Throughout the course, you will learn the following topics:

1. Introduction to Version Control
   - Understanding the need for version control
   - Git's advantages and key concepts

2. Setting Up Git
   - Installing Git on different platforms (Windows, macOS, Linux)
   - Configuring Git with your user information

3. Git Basics
   - Creating a new Git repository
   - Staging and committing changes
   - Understanding the Git workflow

4. Branching and Merging
   - Creating branches for new features or bug fixes
   - Merging branches back to the main branch

5. Collaborating with Git
   - Working with remote repositories
   - Pushing and pulling changes from remote branches
   - Resolving merge conflicts

6. Advanced Git Techniques
   - Managing tags and releases
   - Using Git rebase
   - Stashing changes for later use

7. Best Practices and Tips
   - Git workflows and strategies
   - Handling large repositories
   - Troubleshooting common issues

## Prerequisites

To make the most of this course, you should have a basic understanding 
of command-line interfaces and programming concepts. Familiarity with 
any programming language will be beneficial, but it's not mandatory.

## Getting Started

1. Clone this repository to your local machine.
2. Install Git following the instructions in the course materials.
3. Explore the course materials, exercises, and examples provided.

## Course Resources

- Course materials and exercises can be found in this repository.
- Join our community forum to connect with other learners and get 
help when needed.

## Certification

Upon completing the course, you'll receive a certificate of completion 
to showcase your newfound Git skills.

# Git Code with Mosh

## Git Status 

```
git status -s
```

The `git status -s` command is a short and concise way to view the
status of your Git repository in a simplified and easy-to-read format.
It provides a summary of the changes between the current state of your repository's __working tree__ and the __staging area__.

When you run `git status -s`, you will see output that looks like this:

```
 M file1.txt
MM file2.txt
A  file3.txt
?? new_file.txt
```

The status output is organized into columns:

1. The __first column__ represents the status of the __staging area__.
2. The __second column__ represents the status of the __working tree__.

Here's the meaning of the possible status codes:

- `??`: Untracked files - Files that are present in the working tree
but not yet tracked by Git (not added to the staging area).

- `A`: New file addition - A new file has been added to the staging area.

- `M`: File modification - A file has been modified in the working tree,
and the changes are staged and ready to be committed.

- `D`: File deletion - A file has been deleted in the working tree,
and the deletion is staged and ready to be committed.

- `R`: File rename - A file has been renamed in the working tree,
and the rename is staged and ready to be committed.

- `C`: File copy - A file has been copied in the working tree,
and the copy is staged and ready to be committed.

- `U`: Conflict - A merge conflict exists in the file between the branch
you are on and the branch you are merging or rebasing.

The absence of any letter in the first column indicates that the file's
status in the staging area has not changed since the last commit.

The absence of any letter in the second column indicates that the file's
status in the working tree has not changed since the last commit.

## git show

The `git show` command is a versatile tool in Git that is used to view 
expanded details on Git objects such as blobs, trees, tags, and commits. 
Here's a breakdown of what it does:

- **Commits**: It shows the log message and textual diff. It also presents 
the merge commit in a special format as produced by `git diff-tree --cc`.
- **Tags**: It shows the tag message and the referenced objects¹.
- **Trees**: It shows the names (equivalent to `git ls-tree` with `--name-only`).
- **Blobs**: It shows the plain contents.

The command takes options applicable to the `git diff-tree` command to 
control how the changes the commit introduces are shown¹. By default, 
`git-show` acts against the `HEAD` reference, which always points to 
the last commit of the current branch. Therefore, you can use 
`git-show` to display the log message and diff output of the latest 
commit.

There are several options you can use with `git show` to customize its 
output, such as:
- `--pretty[=<format>]`: Pretty-print the contents of the commit logs 
in a given format.
- `--abbrev-commit`: Instead of showing the full 40-byte hexadecimal 
commit object name, show a prefix that names the object uniquely.
- `--no-abbrev-commit`: Show the full 40-byte hexadecimal commit object name.
- `--oneline`: This is a shorthand for `--pretty=oneline --abbrev-commit` 
used together.
- `--encoding=<encoding>`: Re-code the commit log message in the encoding 
preferred by the user.
- `--expand-tabs=<n>`, `--expand-tabs`, `--no-expand-tabs`: Perform a tab 
expansion (replace each tab with enough spaces to fill to the next 
display column that is multiple of `<n>`) in the log message 
before showing it in the output.

This command is quite useful when you want to examine the details of 
specific objects in your Git repository.

----
The `git show` command is used to view detailed information about Git objects,
including blobs, trees, tags, and commits. It is similar to the `git log` command, but it provides more detail about each object.

When used to view a commit, `git show` displays the following information:

* The commit hash
* The author name and email address
* The commit date and time
* The commit message
* A diff of the changes introduced by the commit

`git show` can also be used to view specific files within a commit,
or to view a range of commits. For example, to view the changes to the file
 `README.md` in the most recent commit, you would use the following command:


```
git show README.md
```

To view all of the commits in the `master` branch that were made by the user
`john.doe`, you would use the following command:

```
git show master --author=john.doe
```

`git show` is a powerful tool for examining the history of a Git repository. 
It can be used to troubleshoot problems, track down changes, and learn 
more about how a project has evolved over time.

Here are some examples of how `git show` can be used:

* To find the commit that introduced a particular bug:

```
git show --before=bug-fix-commit --after=buggy-commit
```

* To track down the changes to a specific file over time:

```
git show --name-only <file-name>
```

* To see how a commit message has evolved:

```
git show --pretty=format:"%h %s" --first-parent <commit-hash>
```

`git show` is a versatile command with many uses. It is a valuable tool for any Git user.


##  git ls-files

The git ls-files command lists the files that are tracked by Git.
This includes files that are in the index, as well as files that are
in the working tree but not in the index.

```
git ls-files

```

Here are some of the most commonly used options for git ls-files:

|Option|Effect|
|------|------|
|-c | Show the file mode.|
|-z | Show the filenames verbatim.|
|-i | Show only ignored files.|
|--stage | Show the stage information for each file.|
|--unmerged | Show unmerged files.|
|--deleted | Show deleted files.|
|--others | Show files that are not tracked by Git.|


## git ls-tree

The `git ls-tree` command is used to display the content of a specific
Git tree object. In Git, a tree object represents a directory or a
subdirectory within the repository, and it stores references to other
tree objects or blob objects (files) along with their associated metadata.

The basic syntax of the `git ls-tree` command is as follows:

```bash
git ls-tree [<commit>] [<path>]
```

- `<commit>`: Optional. The commit hash or reference to the commit that
contains the tree object you want to list. If not specified, it
defaults to the current commit (HEAD).

- `<path>`: Optional. The path to a specific subdirectory or file
within the tree object. If provided, the command will display the
contents of the tree at the specified path. If omitted, it shows the
entire tree object.

Let's explore some examples:

1. To list the contents of the current tree (current commit):

```bash
git ls-tree HEAD
```

2. To list the contents of a tree in a specific commit:

```bash
git ls-tree <commit-hash>
```

3. To list the contents of a subdirectory within a tree:

```bash
git ls-tree HEAD path/to/subdirectory
```

The output of the `git ls-tree` command displays information about
each entry in the tree. The format of the output is:

```
<mode> <type> <object>	<file/path>
```

- `<mode>`: The file mode of the entry, which represents the
permissions and object type
(e.g., 100644 for a regular file, 040000 for a subdirectory).

- `<type>`: The type of the entry, which can be "blob" for a file
or "tree" for a subdirectory.

- `<object>`: The SHA-1 hash of the object (either blob or tree)
associated with the entry.

- `<file/path>`: The relative path to the file or subdirectory
within the tree.

The `git ls-tree` command is particularly useful for inspecting the
contents of a tree object in Git, such as when you need to verify
the files and directories present in a specific commit or tree.
It is often used in combination with other Git commands to examine
the repository's history and track changes to files and directories
over time.


## Restore a file

The `git restore` command is used to restore files in your working tree
to a previous state. It allows you to undo changes made to files,
revert modifications, or even discard uncommitted changes and restore
them to the state they were in at a specific commit or in the
staging area.

The basic syntax of the `git restore` command is as follows:

```bash
git restore <file-path>
```

This will restore the specified file in the working tree to the version
found in the __staging area__. Any changes made to the file since the
last `git add` (staging) will be discarded.

You can also use `git restore` with additional options to restore files
from different sources:

1. **Restore a file to a specific commit:**

   ```bash
   git restore --source=<commit> <file-path>
   ```

   This command restores the specified file to the version found in the
   given commit. The changes made to the file since that commit will
   be discarded.

2. **Restore a file to a specific branch or commit reference:**

   ```bash
   git restore --source=<branch/commit> --staged <file-path>
   ```

   This command restores the specified file to the version found in
   the specified branch or commit. The restored version will be added
   to the staging area, allowing you to create a new commit with
   the restored changes.

3. **Restore all files in the working tree to a specific commit:**

   ```bash
   git restore --source=<commit> .
   ```

   This command restores all files in the working tree to the versions
   found in the given commit. This effectively reverts the entire
   working tree to the state it was in at that commit.

It's important to note that `git restore` is used to work with files in
the __working tree__ and the __staging area____. It does not affect
commits in the repository's history. If you want to undo a commit and
remove it from the history, you should use commands like
`git reset`, `git revert`, or `git cherry-pick`.

Be cautious when using `git restore`, especially with the `--source`
option, as it discards changes in the working tree and cannot be undone.
It is recommended to create a backup or use Git's branching and tagging
features before performing any major restoration actions.

[Git code with Mosh]: https://codewithmosh.com/p/the-ultimate-git-course

