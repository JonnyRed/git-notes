# GitHub Notes

A set of cheat sheet Git notes that I find useful in my usage of
Git.

## Table of Contents

- [Introduction](#introduction)
- [Content](#content)
- [Introduction to Git and GitHub](#introduction-to-git-and-github)
- [Git Code with Mosh][]

---

## Git Quick Notes

### Introduction

Welcome to my collection of Git quick notes! As I navigate my way through Git and its various intricacies, I often find myself forgetting certain aspects or commands. These notes serve as a compilation of the valuable bits and pieces that I come across and want to remember for future reference.

In this repository, you'll find a collection of concise and practical notes that I've gathered while working with Git. These notes aim to provide quick reminders, helpful tips, and useful snippets that can assist both beginners and experienced users in their Git journeys.

Please note that these are personal notes, so they reflect my own experiences and preferences. If you find any errors, I encourage you to open an issue or submit a pull request.

### Content

1. Git Configuration:
   - `git config --global user.name "John Reynolds"`: Sets up Git with 
   your name.
   - `git config --global user.email "jjmreynolds@gmail.com"`: Sets up Git 
   with your email.
   - `git config --global color.ui auto`: Makes sure that Git output is coloured.
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

### Introduction to Git and GitHub

[Introduction to Git and GitHub][] teaches you the basics of Git, 
a version control system, and GitHub, a web-based hosting service for 
Git repositories. The course covers topics such as creating and cloning 
repositories, working with branches, and resolving conflicts. 
It also includes hands-on labs that allow you to practice what 
you've learned.

The course is divided into three weeks.

- Week 1, you'll learn about the basics of Git and GitHub. You'll create
your first repository and clone it onto your computer. 
You'll also learn about branches and how to use them to track changes 
to your code.
- Week 2, you'll learn more about working with branches. You'll learn 
how to merge branches and how to resolve conflicts. 
You'll also learn about remote repositories and how to push and pull 
changes from them.
- Week 3, you'll learn about some advanced Git concepts. You'll learn 
about tags, which are used to mark specific points in your code history. 
You'll also learn about rebasing and merging, which are two ways to 
change the history of your code.

- Week 1, you'll learn about the basics of Git and GitHub. You'll create
your first repository and clone it onto your computer.
You'll also learn about branches and how to use them to track changes
to your code.

- Week 2, you'll learn more about working with branches. You'll learn
how to merge branches and how to resolve conflicts.
You'll also learn about remote repositories and how to push and pull
changes from them.
- Week 3, you'll learn about some advanced Git concepts. You'll learn
about tags, which are used to mark specific points in your code history.
You'll also learn about rebasing and merging, which are two ways to
change the history of your code.

[Introduction to Git and GitHub]:https://www.coursera.org/learn/introduction-git-github/home/week/1

## The Ultimate Git Course

Welcome to **The Ultimate Git Course**! This comprehensive course will 
take you from a beginner to a proficient user of Git, the industry-standard 
version control system. Whether you're a developer, designer, or any 
other professional working with code or files, mastering Git is essential 
for efficient collaboration and project management.

### Course Overview

This course is designed to provide a hands-on learning experience, 
with practical examples and exercises to reinforce your understanding. 
You'll be guided by our experienced instructor, 
Mosh Hamedani, who has a passion for teaching and a wealth of expertise 
in software development.

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

### Prerequisites

To make the most of this course, you should have a basic understanding 
of command-line interfaces and programming concepts. Familiarity with 
any programming language will be beneficial, but it's not mandatory.

### Getting Started

1. Clone this repository to your local machine.
2. Install Git following the instructions in the course materials.
3. Explore the course materials, exercises, and examples provided.

### Course Resources

- Course materials and exercises can be found in this repository.
- Join our community forum to connect with other learners and get 
help when needed.

### Certification

Upon completing the course, you'll receive a certificate of completion 
to showcase your newfound Git skills.

## Git Code with Mosh

### Git Status

```bash
git status -s
```

The `git status -s` command is a short and concise way to view the
status of your Git repository in a simplified and easy-to-read format.
It provides a summary of the changes between the current state of your repository's **working tree** and the **staging area**.

When you run `git status -s`, you will see output that looks like this:

```text
 M file1.txt
MM file2.txt
A  file3.txt
?? new_file.txt
```

The status output is organized into columns:

1. The **first column** represents the status of the **staging area**.
2. The **second column** represents the status of the **working tree**.

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

The `git show` command is used to view detailed information about 
Git objects, including blobs, trees, tags, and commits. 
It is similar to the `git log` command, but it provides more detail 
about each object.

When used to view a commit, `git show` displays the following information:

- The commit hash
- The author name and email address
- The commit date and time
- The commit message
- A diff of the changes introduced by the commit

`git show` can also be used to view specific files within a commit,
or to view a range of commits. For example, to view the changes to the file
 `README.md` in the most recent commit, you would use the following command:


```bash
git show README.md
```

To view all of the commits in the `master` branch that were made by the user
`john.doe`, you would use the following command:

```bash
git show master --author=john.doe
```

`git show` is a powerful tool for examining the history of a Git repository. 
It can be used to troubleshoot problems, track down changes, and learn 
more about how a project has evolved over time.

Here are some examples of how `git show` can be used:

- To find the commit that introduced a particular bug:

```bash
git show --before=bug-fix-commit --after=buggy-commit
```

- To track down the changes to a specific file over time:

```bash
git show --name-only <file-name>
```

- To see how a commit message has evolved:

```bash
git show --pretty=format:"%h %s" --first-parent <commit-hash>
```

`git show` is a versatile command with many uses. It is a valuable tool for any Git user.

### git show1

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

The `git show` command is used to view detailed information about
Git objects, including blobs, trees, tags, and commits.
It is similar to the `git log` command, but it provides more detail
about each object.

When used to view a commit, `git show` displays the following information:

- The commit hash
- The author name and email address
- The commit date and time
- The commit message
- A diff of the changes introduced by the commit

`git show` can also be used to view specific files within a commit,
or to view a range of commits. For example, to view the changes to the file
 `README.md` in the most recent commit, you would use the following command:

```bash
git show README.md
```

To view all of the commits in the `master` branch that were made by the user
`john.doe`, you would use the following command:

```bash
git show master --author=john.doe
```

`git show` is a powerful tool for examining the history of a Git repository.
It can be used to troubleshoot problems, track down changes, and learn
more about how a project has evolved over time.

Here are some examples of how `git show` can be used:

- To find the commit that introduced a particular bug:

```bash
git show --before=bug-fix-commit --after=buggy-commit
```

- To track down the changes to a specific file over time:

```bash
git show --name-only <file-name>
```

- To see how a commit message has evolved:

```bash
git show --pretty=format:"%h %s" --first-parent <commit-hash>
```

`git show` is a versatile command with many uses. It is a valuable tool for any Git user.

### git ls-files

The git ls-files command lists the files that are tracked by Git.
This includes files that are in the index, as well as files that are
in the working tree but not in the index.

```bash
git ls-files

```

Here are some of the most commonly used options for git ls-files:

| Option     | Effect                                    |
|------------|-------------------------------------------|
| -c         | Show the file mode.                       |
| -z         | Show the filenames verbatim.              |
| -i         | Show only ignored files.                  |
| --stage    | Show the stage information for each file. |
| --unmerged | Show unmerged files.                      |
| --deleted  | Show deleted files.                       |
| --others   | Show files that are not tracked by Git.   |

### git ls-tree

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

```text
<mode> <type> <object> <file/path>
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

### git show2

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

The `git show` command is used to view detailed information about Git objects,
including blobs, trees, tags, and commits. It is similar to the `git log` 
command, but it provides more detail about each object.

When used to view a commit, `git show` displays the following information:

- The commit hash
- The author name and email address
- The commit date and time
- The commit message
- A diff of the changes introduced by the commit

`git show` can also be used to view specific files within a commit,
or to view a range of commits. For example, to view the changes to the file
 `README.md` in the most recent commit, you would use the following command:

```bash
git show README.md
```

To view all of the commits in the `master` branch that were made by the user
`john.doe`, you would use the following command:

```bash
git show master --author=john.doe
```

`git show` is a powerful tool for examining the history of a Git repository.
It can be used to troubleshoot problems, track down changes, and learn
more about how a project has evolved over time.

Here are some examples of how `git show` can be used:

- To find the commit that introduced a particular bug:

```bash
git show --before=bug-fix-commit --after=buggy-commit
```

- To track down the changes to a specific file over time:

```bash
git show --name-only <file-name>
```

- To see how a commit message has evolved:

```bash
git show --pretty=format:"%h %s" --first-parent <commit-hash>
```

`git show` is a versatile command with many uses. It is a valuable tool for any Git user.

### Restore a file

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
found in the **staging area**. Any changes made to the file since the
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
the **working tree** and the **staging area**__. It does not affect
commits in the repository's history. If you want to undo a commit and
remove it from the history, you should use commands like
`git reset`, `git revert`, or `git cherry-pick`.

Be cautious when using `git restore`, especially with the `--source`
option, as it discards changes in the working tree and cannot be undone.
It is recommended to create a backup or use Git's branching and tagging
features before performing any major restoration actions.

## Git `clean`

The `git clean` command is used to remove untracked files and directories 
from the working tree¹. Untracked files are files that have been created 
within your repo's working directory but have not yet been added to the 
repository's tracking index using the `git add` command⁴. 

Here are some common options for `git clean`:

- `-n`: This option performs a “dry run” of `git clean`. It shows you 
which files are going to be removed without actually removing them.
- `-f`: This option forces the deletion of untracked files.
- `-d`: This option removes untracked directories.
- `-x`: This option removes ignored files.
- `-i`: This option allows you to do an interactive clean.

For example, if you want to see which files will be removed without 
actually removing them, you can use the `-n` option like this: `git clean -n`.

Please note that when fully executed, `git clean` will make a hard filesystem 
deletion, similar to executing the command line `rm` utility. Make sure you 
really want to delete the untracked files before you run it.

## Browsing History

### git log --oneline --stat

The `git log --oneline --stat` command is a combination of two options 
with the `git log` command in Git, a distributed version control system. 
Here's what each part does:

- `git log`: This command shows the commit history in reverse chronological 
order. The commits are displayed starting from the most recent commit.

- `--oneline`: This is an option for `git log` that changes the output 
format to be more compact. Each commit is shown as one line containing 
the commit hash and the commit message.

- `--stat`: This option shows some stats about each commit, specifically, 
it shows which files were altered and the relative number of lines that 
were added or deleted from each of them.

So, when you use `git log --oneline --stat`, Git will display each 
commit as a single line with its hash and message, followed by stats 
about which files were changed and how many lines were added or deleted 
in that commit. It's a useful command for getting a high-level overview 
of your project history.


### git log --oneline --patch

- `--patch` or `-p`: This option generates patch text for each commit. 
The patch text shows the actual changes in content that were made in each 
commit, line by line.

So, when you use `git log --oneline --patch`, Git will display each 
commit as a single line with its hash and message, followed by the actual 
changes made in that commit, line by line. It's a useful command for 
reviewing your project history in detail.

### git log --oneline -\<integer\>

The last three commits for example:

`git log --oneline -3`

### git log --oneline --author=\<Name\>

Filter by author 

`git log --oneline --author="John Reynolds"`

### git log --oneline --after="YYYY-MM-DD"

Examples of date filtering:

`git log --oneline --after="2022-05-01"`
`git log --oneline --after="yesterday"`
`git log --oneline --after="one week ago"`

### git log --oneline --grep="commit string"

- `--grep="commit string:"`: This option makes `git log` only show 
__commits__ where the commit message contains the string `"commit string:"`. 
The `--grep` option is followed by a string, and it causes `git log` 
__to only list commits__ where that string appears in the commit message.

### git log --oneline -S="string"

- `-S"string"`: This option makes `git log` only show commits that added or
removed the string `"string"`. The `-S` option is followed by a string, 
and it causes `git log` to only list commits where that string was 
added or removed from the codebase.


### git log --oneline \<commit id>..\<commit id>

The `git log --oneline commit_id..commit_id` command in Git shows the 
commit history between the two specified commit IDs in a compact format. 

- `commit_id..commit_id`: This is a range of commits. Git will show all 
commits that exist in the second commit ID which don't exist in the first 
commit ID. In other words, it shows the commits that happened between these 
two points in the history.

So, when you use `git log --oneline commit_id..commit_id`, Git will 
display each commit as a single line with its hash and message, 
but only for commits that are in the range between the two specified 
commit IDs. It's a useful command for reviewing a specific part of 
your project history.

### git log --oneline \<filename>

- `filename`: This is the name of a file in your repository. When you 
specify a filename after `git log`, Git will only show commits where 
that file was changed.

So, when you use `git log --oneline filename`, Git will display each 
commit as a single line with its hash and message, but only for commits 
where the specified file was changed. It's a useful command for seeing 
how a specific file has changed over time.

### Git Log format

#### git log --pretty=format:\<format string>

Example:

`git log --pretty=format:"%an committed %h"`

### Alias

Example 

`git config --global alias.lg "log --pretty=format:'%an committed %h on %cd'"`

`git config --global -e`

### git shortlog

The `git shortlog` command in Git is used to summarize the output of `git log`. 
It takes the same arguments as `git log`, but instead of displaying the 
full commit messages, it groups the commits by author and title, 
making it easy to see who has done what in a repository.

Here's a basic breakdown of what it does:

- `git shortlog`: This command summarizes the output of `git log`. 
It groups the commits by author and then by commit title.

This is a useful command when you want to get a quick overview of who has 
been committing to your repository and what they've been doing. 
It's often used in open source projects to generate a list of contributions 
for release notes or other documentation.

### git squash merge

In Git, a squash merge is a merge option that allows you to condense the 
Git history of feature branches when you complete a merge. Using the 
`git merge --squash` command, you can create a single commit on your 
main branch with the changes from a feature branch as opposed to having
 all commits from that feature branch added to the history.

Here's a step-by-step breakdown of how it works:

1. **Checkout to the branch you want to merge into**: This is usually 
your main or master branch. You can do this with `git checkout main`.

2. **Perform the squash merge**: You can do this with 
`git merge --squash feature_branch`, where `feature_branch` is the 
name of the branch that contains your new feature.

3. **Commit the changes**: After a squash merge, you'll have all the 
changes from your feature branch staged on your main branch, 
but they aren't committed yet. You can commit them with `git commit`.

The result is that your feature branch's history is left intact, but 
when you look at the history of your main branch, it looks like one 
single commit was made with all the changes from your feature branch. 
This can be useful for keeping your main branch history clean and 
understandable.

It's important to note that squash merging is a one-way operation. 
Once it's done, there's no easy way to go back and get the individual 
commits from a squashed branch. So it's a good idea to be sure about 
using this option before you do it.

### git rebase

In Git, `rebase` is a command that allows you to integrate changes from 
one branch into another. It's an alternative to the `git merge` command. 
The primary reason to use `rebase` is to maintain a linear project history.

Here's a step-by-step breakdown of how it works:

1. **Checkout to the branch you want to rebase**: This is usually your 
feature branch that you want to update with changes from the main branch. 
You can do this with `git checkout feature_branch`.

2. **Perform the rebase**: You can do this with `git rebase main`, where 
`main` is the branch that has the new commits you want to include in your 
feature branch.

The result is that your feature branch will be rewritten as if it was based 
on the head of the main branch, as opposed to the commit it was actually 
based on. This makes your feature branch up-to-date with the latest code 
on the main branch.

During a rebase, conflicts may arise if there are changes in both branches 
that touch the same parts of the code. Git will pause and allow you to resolve 
those conflicts manually. Once resolved, you can continue the rebase with 
`git rebase --continue`.

It's important to note that because `rebase` changes the commit history 
by creating new commits for each commit in the original branch, 
it should be used with caution. It's generally recommended not to use 
`rebase` on public branches that others are working on.

Remember, always create a backup or use a temporary branch when performing 
operations that rewrite history (like `git rebase`) if you're unsure 
about the process.

### git cherry-pick

In Git, `cherry-pick` is a powerful command that enables arbitrary Git 
commits to be picked by reference and appended to the current working HEAD. 
Cherry picking is the act of picking a commit from a branch and applying 
it to another.

Here's a step-by-step breakdown of how it works:

1. **Identify the commit you want to pick**: This is usually done by looking 
at the log of another branch with `git log`.

2. **Apply the commit**: You can do this with `git cherry-pick commit_id`, 
where `commit_id` is the hash of the commit you want to apply.

The result is that the changes introduced by the specified commit are 
applied to your current branch. A new commit is created with this change, 
and your branch's history remains linear.

It's important to note that cherry picking only applies the changes introduced 
by the commit you pick, not the entire state of the repository at that commit. 
Changes made in other commits are not included.

Cherry picking can be very useful when you want to get some useful work 
from another branch without merging or pulling in all changes from that 
branch. But be careful: cherry picking can sometimes lead to duplicate 
commits and could make your history harder to understand.

### Git `clean1`

The `git clean` command is used to remove untracked files and directories
from the working tree¹. Untracked files are files that have been created
within your repo's working directory but have not yet been added to the
repository's tracking index using the `git add` command⁴.

Here are some common options for `git clean`:

- `-n`: This option performs a “dry run” of `git clean`. It shows you
which files are going to be removed without actually removing them.
- `-f`: This option forces the deletion of untracked files.
- `-d`: This option removes untracked directories.
- `-x`: This option removes ignored files.
- `-i`: This option allows you to do an interactive clean.

For example, if you want to see which files will be removed without
actually removing them, you can use the `-n` option like this: `git clean -n`.

Please note that when fully executed, `git clean` will make a hard filesystem
deletion, similar to executing the command line `rm` utility. Make sure you
really want to delete the untracked files before you run it.
