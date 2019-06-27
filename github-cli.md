**Quick Tip: Github and Command Line Interface (CLI)**
======

## **Overview**
This is a quick guide to help you learn the basics about Github and CLI! If you have any more questions, or want other resources, [click here](https://www.atlassian.com/git/tutorials) for a good reference regarding Github and [ here](https://tutorial.djangogirls.org/en/intro_to_command_line/) for a good reference regarding CLI.

## **Command Line Interface**
<img src="https://memegenerator.net/img/instances/65841187/turn-off-the-gui-luke-use-the-command-line.jpg" width="300px" height="300px"/>

### Introduction
**What: ** CLI is a text-based interface which can be accessed through terminal (for OS X and Linux) or command prompt (for Windows). It allows a user to interact with the operating system seamlessly.

**Why: ** While the Graphical User Interface (GUI) allows for editing and accessing files and folders, the CLI gives the user more power and precision.

**NOTE: ** Some commands  are different for OS X and Linux vs Windows. Make sure you're using the right ones!

### Commands

#### Current Directory

**OS X and Linux: ** `pwd` stands for "print working directory"

**Windows: ** `cd` stands for "change directory" and can be used to switch to a new directory as well

#### Learn More About a Command
**OS X and Linux: ** `man <command>`

**Windows: ** `<command> /?`

#### List Files and Directories
**OS X and Linux: ** `ls`

**Windows: ** `dir`

#### Change Current Directory
**OS X, Linux, and Windows: ** `cd <path>`

#### Move to the Parent Directory
**OS X, Linux, and Windows: ** `cd ..`

#### Create Directory
**OS X, Linux, and Windows: ** `mkdir <name of directory>`

### Cheat Sheet
| Command | OS X and Linux | Windows |
| :-----: | :------------: | :-----: |
| Current Directory | `pwd` |  `cd`  |
| Learn More | `man <command>` | `<command> /?` |
| List Files and Directories | `ls` | `dir` |
| Change Current Directory | `cd <path>` | `cd <path` |
| Move to Parent Directory | `cd ..` | `cd ..` |
| Create Directory | `mkdir <name of directory`> | `mkdir <name of directory>` |


## **Github**
<img src="https://memegenerator.net/img/instances/41740049/regular-peopleadd-me-on-facebook-me-fork-me-on-github.jpg" width="300px" height="300px"/>

### Introduction
**What: ** Git is a version control system which allows multiple people to work on a project at the same time (kind of like Google Docs).

**Why: ** Imagine cooking with your friends: you all have to keep track of what the others are adding to the dish while making sure that what you add doesn't ruin it. Things get more complicated as more and more people join. The same is true of technical projects.

**How: ** [Github!](https://github.com/)

### Commands
#### `git init <repository name`
This will create a new git repository on your **local** machine

#### `git clone <link to Github repository>`
This allows you to create a copy of the project on your local machine. When you make changes, they'll only show up on your copy, we'll talk about how to **push** your changes to the remote repository in another command

#### `git checkout [-b <new branch name> | <existing branch>]`
<img src="https://wac-cdn.atlassian.com/dam/jcr:86eba9ec-9391-45ea-800a-948cec1f2ed7/Branch-2.png?cdnVersion=lf" width="400px" height="300px"/>

Branching is useful when you want to add a feature to the project without affecting the code of others working on it. It allows you to work on your feature without worrying about what others are working on *for now*

#### `git add [<file/directory> | .]`
Adding a file means that you want to move a file from the working directory to the staging directory. These files will be added to the next **commit** which will be explained in the next command. **Note: ** `git add .` indicates that you want to add all the files you just updated to the staging directory.

#### `git commit -m "<commit message>"`
This command is used to save the changes you made in your local repository. The commit message is often a sentence or two explaining what you changed and why.

#### `git status`
This command will show you what branch you're on, tracked and untracked files, and which files are staged for a commit.

#### `git push origin <branch name>`
This command is used to update the remote repository (on Github) with the changes you just made on your local repository.

#### `git pull origin <branch name>`
This allows you to update your local copy of the repository with any changes others updated the remote repository with. **Do this every now and then so that your branch is not completely outdated**

#### `git rebase <branch>`
Sometimes more than one person will edit the same file and a **merge conflict** will occur. Use this command to choose which and whose changes you want to include in your file.

#### `git merge <branch name>`
This command will allow you to combine two branches together. **BE CAREFUL!!! You typically want at least one other person to check over your code to make sure that your changes don't break the project**

### Cheat Sheet
| Command | Meaning |
| :-----: | :-----: |
| `git init <repository name> ` | Create a new repository |
| `git clone <link to Github repository>` | Get a local copy of a Github repository |
| `git checkout [-b <new branch name> `<code>&#124;</code>`<existing branch>]` | Switch to a new branch |
| `git add [<file/directory> `<code>&#124;</code>` .]` | Move files from working directory to staging |
| `git commit -m "<commit message>"` | Save your changes on your local machine |
| `git status` | View the status of your project |
| `git push origin <branch name>` | Update the remote repository with your local changes |
| `git pull origin <branch name>` | Update your local repository with remote changes |
| `git rebase <branch>` | Used to fix merge conflicts |
| `git merge <branch name>` | Combine two branches together |
