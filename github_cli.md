**Quick Tip: Github and Command Line Interface (CLI)**
======
_Written by Stephanie Almeida, for HackGT_

## **Overview**
This is a quick guide to help you learn the basics about Github and CLI! If you have any more questions, or want other resources, [click here](https://tutorial.djangogirls.org/en/intro_to_command_line/) for a good reference regarding CLI and [ here](https://www.atlassian.com/git/tutorials) for a good reference regarding Github.

## **Command Line Interface**
<img src="https://memegenerator.net/img/instances/65841187/turn-off-the-gui-luke-use-the-command-line.jpg" width="300px" height="300px"/>

### Introduction
**What:** CLI is a text-based interface which can be accessed through terminal (for OS X and Linux) or command prompt (for Windows). It allows a user to interact with the operating system seamlessly. Bash is the shell language which is used for OS X and Linux. It is also available for Windows, but it is not the default.

**Why:** While the Graphical User Interface (GUI) allows for editing and accessing files and folders, the CLI gives the user more power and precision.

**NOTE:** Some commands  are different for OS X and Linux vs Windows. Make sure you're using the right ones!

### Commands

#### Current Directory

**OS X and Linux:** `pwd` stands for "print working directory"

**Windows:** `cd` stands for "change directory" and can be used to switch to a new directory

#### Learn More About a Command
**OS X and Linux:** `man <command>` is short for manual so `man pwd` would tell you more about the `pwd` command

**Windows:** `<command> /?`

#### List Files and Directories
**OS X and Linux:** `ls`

**Windows:** `dir`

#### Change Current Directory
**OS X, Linux, and Windows:** `cd <path>`

#### Move to the Parent Directory
**OS X, Linux, and Windows:** `cd ..`

#### Create Directory
**OS X, Linux, and Windows:** `mkdir <name of directory>`

#### Remove Empty Directories
**OS X, Linux, and Windows:** `rmdir <empty directory>`

#### Remove Directories
**OS X, Linux, and Windows:** `rm -rf <directory>` **Note:** This recursively removes all files and directories so *be careful*


#### Change Permissions
**OS X and Linux:** `chmod` [More info](https://ss64.com/bash/chmod.html)

**Windows:** No true equivalent :(

#### Running an Executable
**OS X and Linux:** `./<filename>`

**Windows:** `start <filename>.exe`

#### Autocomplete
**OS X, Linux, and Windows:** `[tab]`

#### Go to Beginning of Line
**OS X, Linux, and Windows:** `ctrl-a`

#### Go to End of Line
**OS X, Linux, and Windows:** `ctrl-e`

### Cheat Sheet
| Command | OS X and Linux | Windows |
| :-----: | :------------: | :-----: |
| Current Directory | `pwd` |  `cd`  |
| Learn More | `man <command>` | `<command> /?` |
| List Files and Directories | `ls` | `dir` |
| Change Current Directory | `cd <path>` | `cd <path` |
| Move to Parent Directory | `cd ..` | `cd ..` |
| Create Directory | `mkdir <name of directory`> | `mkdir <name of directory>` |
| Remove Empty Directory | `rmdir <empty directory>` | `rmdir <empty directory>` |
| Remove Directories | `rm -rf <directory>` | `rm -rf <directory>` |
| Change Permissions | `chmod` | none :( |
| Running an Executable | `./<filename>` | `start <filename>.exe` |
| Autocomplete | `[tab]` | `[tab]` |
| Go to Beginning of Line | `ctrl-a` | `ctrl-a` |
| Go to End of Line | `ctrl-e` | `ctrl-e` |

## **Github**
<img src="https://memegenerator.net/img/instances/41740049/regular-peopleadd-me-on-facebook-me-fork-me-on-github.jpg" width="300px" height="300px"/>

### Introduction
**What:** Git is a version control system which allows multiple people to work on a project at the same time (kind of like Google Docs).

**Why:** Imagine cooking with your friends: you all have to keep track of what the others are adding to the dish while making sure that what you add doesn't ruin it. Things get more complicated as more and more people join. The same is true of technical projects.

**How:** [Github!](https://github.com/) is the primary host of git projects, but as a concept, git exists by itself as well.

### Commands
#### `git init <repository name>`
This will create a new git repository on your **local** machine. You can also create a new git repository on Github itself using their GUI. [More info](https://www.google.com/url?sa=t&rct=j&q=&esrc=s&source=web&cd=1&cad=rja&uact=8&ved=2ahUKEwjczsGh75HjAhWGhOAKHUH1AuoQFjAAegQIBBAB&url=https%3A%2F%2Fwww.atlassian.com%2Fgit%2Ftutorials%2Fsetting-up-a-repository%2Fgit-init&usg=AOvVaw0wJ8DN5PYMXq1i8IpC98Xw)

#### `git clone <link to Github repository>`
This allows you to create a copy of the project on your local machine. When you make changes, they'll only show up on your copy, we'll talk about how to **push** your changes to the remote repository in another command. [More info](https://www.google.com/url?sa=t&rct=j&q=&esrc=s&source=web&cd=1&cad=rja&uact=8&ved=2ahUKEwidz92t75HjAhXunuAKHYrdBx8QFjAAegQICBAC&url=https%3A%2F%2Fwww.atlassian.com%2Fgit%2Ftutorials%2Fsetting-up-a-repository%2Fgit-clone&usg=AOvVaw2J2FfedigWA32-5jmLH7kR)

#### `git checkout [-b <new branch name> | <existing branch>]`
<img src="https://wac-cdn.atlassian.com/dam/jcr:86eba9ec-9391-45ea-800a-948cec1f2ed7/Branch-2.png?cdnVersion=lf" width="400px" height="300px"/>

Branching is useful when you want to add a feature to the project without affecting the code of others working on it. It allows you to work on your feature without worrying about what others are working on *for now*. Master is the default branch. [More info](https://www.google.com/url?sa=t&rct=j&q=&esrc=s&source=web&cd=1&cad=rja&uact=8&ved=2ahUKEwjSxOa975HjAhXQct8KHY_2B5IQFjAAegQICBAC&url=https%3A%2F%2Fwww.atlassian.com%2Fgit%2Ftutorials%2Fusing-branches%2Fgit-checkout&usg=AOvVaw0z8S3GUQD1LSLIN37t4Dlw)

#### `git add <file/directory>`
Adding a file means that you want to move a file from the working directory to the staging directory. These files will be added to the next **commit** which will be explained in the next command. [More info](https://www.atlassian.com/git/tutorials/saving-changes)

#### `git commit -m "<commit message>"`
This command is used to save the changes you made in your local repository. The commit message is often a sentence or two explaining what you changed and why. Since commits are stored with reference codes, messages help differentiate between various commits. [More info](https://www.google.com/url?sa=t&rct=j&q=&esrc=s&source=web&cd=1&cad=rja&uact=8&ved=2ahUKEwiq2Lrb75HjAhVknuAKHWiMAmQQFjAAegQIBBAB&url=https%3A%2F%2Fwww.atlassian.com%2Fgit%2Ftutorials%2Fsaving-changes%2Fgit-commit&usg=AOvVaw1DIPPk59HWdSLNQCg2XzqL)

#### `git status`
This command will show you what branch you're on, tracked and untracked files, and which files are staged for a commit. [More info](https://www.google.com/url?sa=t&rct=j&q=&esrc=s&source=web&cd=1&cad=rja&uact=8&ved=2ahUKEwjJ7Lbj75HjAhVihOAKHbEtAgkQFjAAegQIARAB&url=https%3A%2F%2Fwww.atlassian.com%2Fgit%2Ftutorials%2Finspecting-a-repository&usg=AOvVaw1XDLrKXAzAQs74TpVDK3jH)

#### `git push origin <branch name>`
This command is used to update the remote repository (on Github) with the changes you just made on your local repository. If you're pushing to a new branch, git will ask for a head. Use `master` as the upstream. [More info](https://www.google.com/url?sa=t&rct=j&q=&esrc=s&source=web&cd=1&cad=rja&uact=8&ved=2ahUKEwjWsPb-75HjAhVEUt8KHeR6AmMQFjAAegQICBAC&url=https%3A%2F%2Fwww.atlassian.com%2Fgit%2Ftutorials%2Fsyncing%2Fgit-push&usg=AOvVaw3tZOeA6d02P5X_CDKNeWNL)

#### `git pull origin <branch name>`
This allows you to update your local copy of the repository with any changes others updated the remote repository with. **Do this every now and then so that your branch is not completely outdated** [More info](https://www.google.com/url?sa=t&rct=j&q=&esrc=s&source=web&cd=1&cad=rja&uact=8&ved=2ahUKEwi01d2G8JHjAhUnVt8KHYMeDpYQFjAAegQIAxAB&url=https%3A%2F%2Fwww.atlassian.com%2Fgit%2Ftutorials%2Fsyncing%2Fgit-pull&usg=AOvVaw1X-qs2FJetor64yh3lGr4L)

#### `git fetch origin <branch name>`
This command allows you to check out what other have been working on. It's similar to `git pull` but it won't merge the changes together. [More info](https://www.google.com/url?sa=t&rct=j&q=&esrc=s&source=web&cd=2&cad=rja&uact=8&ved=2ahUKEwi9geXr75HjAhUSh-AKHapgAugQFjABegQICxAG&url=https%3A%2F%2Fwww.atlassian.com%2Fgit%2Ftutorials%2Fsyncing%2Fgit-fetch&usg=AOvVaw1KFXUigZOtAtfVkG9xZ39p)

#### `git merge <branch name>`
This command will allow you to combine two branches together. Sometimes more than one person will edit the same file and a **merge conflict** will occur. You'll need to go file be file to fix the conflicts. This is why it is dangerous to merge a branch to master since people assume master has working code. This is why *Pull Requests* exist. **Note: This process is a formality and may be dropped during a hackathon setting. However, it's useful to keep in mind, even if your timescale is only 36 hours.** [More info](https://www.google.com/url?sa=t&rct=j&q=&esrc=s&source=web&cd=1&cad=rja&uact=8&ved=2ahUKEwiCsaWV8JHjAhVkiOAKHdNXAgwQFjAAegQIABAB&url=https%3A%2F%2Fwww.atlassian.com%2Fgit%2Ftutorials%2Fusing-branches%2Fgit-merge&usg=AOvVaw3wzrPRw1lhIveN89ueCB3a)

### Cheat Sheet
| Command | Meaning |
| :-----: | :-----: |
| `git init <repository name> ` | Create a new repository |
| `git clone <link to Github repository>` | Get a local copy of a Github repository |
| `git checkout [-b <new branch name> `<code>&#124;</code>`<existing branch>]` | Switch to a new branch |
| `git add <file/directory>` | Move files from working directory to staging |
| `git commit -m "<commit message>"` | Save your changes on your local machine |
| `git status` | View the status of your project |
| `git push origin <branch name>` | Update the remote repository with your local changes |
| `git pull origin <branch name>` | Update your local repository with remote changes |
| `git fetch origin <branch name>` | See what changes others have been working on |
| `git merge <branch name>` | Combine two branches together |

## Additional Resources
- [CLI](https://tutorial.djangogirls.org/en/intro_to_command_line/)
- [Git, as explained by Github](https://www.atlassian.com/git/tutorials)
- [A Game to Learn git](https://learngitbranching.js.org/?locale=en_US)
