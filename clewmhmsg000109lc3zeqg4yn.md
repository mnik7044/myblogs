---
title: "Let's Get Started With Git."
datePublished: Mon Mar 06 2023 09:31:30 GMT+0000 (Coordinated Universal Time)
cuid: clewmhmsg000109lc3zeqg4yn
slug: lets-get-started-with-git
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1678081400321/8053aa02-1240-4ca3-80dd-885b1c9f89af.png
tags: github, opensource, git, gitcommands, wemakedevs

---

### Introduction

Are you getting started with git ? or an advanced software developer, this guide will help you understand the fundamentals of git and github and how to use them effectively in your software development journey. By the end of this blog, you should have a good understanding of Git and GitHub and be able to manage your projects and collaborate with others with ease.

### What is this git?

Git is nothing but a version control system.

Let's dive into git:

* Imagine you are working on a project and have made some good stuff, but your code breaks after doing some more changes—that's where git comes into play. Git is your time machine for codes you can just go into the past and future and check what changes we made, and when did we make it.
    
* After installing git from the web, we are going to use git bash, which is also a very handy terminal and supports Linux commands as well.
    

### Let's get started

Once you successfully install git in your system, you can get started with it by following the commands below:

You initialize an empty git repository. Here repository stands for your folder.

```bash
git init
```

Firstly, it is important for all of you to understand certain terms before continuing any further.

**Untracked File**\- An untracked file is a file that is not tracked by git, git does not know anything about that file. To track those files we use the command:

```bash
git add <name of the file>
```

Or we can simply track all the files at once by the command:

```bash
git add .
```

**Staged Files**\- Once these files are tracked all these files are ready to be committed, and before committing these changes these files are in the staging area. we can commit the changes by the command:

```bash
git commit -m "Your Message"
```

**Unmodified files**\- Once we commit our changes our file is an unmodified file, we can further change the files by editing them which will ultimately make them modified files.

**Modified files**\- Once we made changes to the file after committing it is certainly known as the modified files. We can send our modified files by adding them to the staging area and again committing them following the previous steps.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1678088260654/c3f19edb-fe2a-4bcd-918d-b1ff19b1d3bd.png align="center")

The image above gives a clear understanding of the given commands.

### Some More Git Commands

git status- This command shows the current status of your repository, including any changes that have been made but not yet committed.

```bash
git status
```

Imagine you made some changes that you don't need and want to match your repo to your last commit, that's where git checkout comes into play.

```bash
git checkout <name of the file>
```

If you want that all files of your repo match the last commit we can use:

```bash
git commit -f
```

Imagine you did a lot of commits and now want to check them, that's when the command git log comes into play, this command shows the commit history of your repository.

```bash
git log
```

Imagine there are a hell lot of commits in your repo and you just want to checkout the last x number of commits, we can do it using:

```bash
git log -p -x
```

Here x is the number of commits that will be shown.

If you want to remove any files from the repo we can do it using:

```bash
git rm <name of the file>
```

If you want to push your repo which you locally created on your local system follow the following commands:

```bash
git remote add origin <link of the github repo>
```

```bash
git push origin master/<name of the branch>
```

### Branches

In Git, a branch is a separate line of development that allows you to make changes to a project without affecting the main branch i.e, the main codebase. It creates a copy of the codebase at a specific point in time and allows you to work on that copy. It can be useful for experimenting with changes without affecting the main codebase until the changes are ready to be merged in.

![Image showing a different branch created named Feature](https://cdn.hashnode.com/res/hashnode/image/upload/v1678095033109/7dc86d08-2b01-4ce0-a7d7-f76437323c6f.png align="center")

**Main/Master branch**\- In git the main/master branch is the default branch that is created when you initialize a new Git repository. It is also the branch that is typically used as the primary branch for a project.

All other branches in the repository can be created off of the main branch and changes made to those branches can eventually be merged back into the main branch when they are ready. In other words, we can say that the main branch is the main trunk of the tree.

**Why should we create multiple branches?**

When multiple developers are working on a project, creating separate branches can help keep changes organized and prevent conflicts. Each developer can work on their own branch and then merge their changes back into the main branch when they are complete without stepping on each other's toes.

**How to create a new branch?**

We can create a new branch by using the following commands:

```bash
git branch <name of the branch>
```

Once we create our branch we need to switch our branch from the main branch to that particular branch. We can do it by using the following command:

```bash
git checkout <name of the branch>
```

But wait, why follow two steps when we can do it one, we can create a branch and directly switch to it by using the following command:

```bash
git checkout -b <name of the branch>
```

To check which branch you are currently on in Git, we can use the command:

```bash
git branch
```

This command lists all the branches in the repository and highlights the currently active branch with an asterisk.

To merge our branch with the master branch we use the command:

```bash
git merge <name of the branch>
```

### What is GitHub?

Assume I am making a project, and my friend wants to work with me on that project, GitHub can help us do that. If git is our code's time machine github can be considered as anywhere door for our code, people from any place can easily collaborate together and contribute to a given project.

GitHub is a web-based hosting platform for Git repositories. It provides a web interface and tools to manage and collaborate on code projects with version control using Git. It is used by developers all around the globe to come together and collaborate.

### How can we get started with open source?

**Forking**\- It will copy the code from the source and will make it a repository under your own account.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1678092031427/d3858b05-6e40-4486-b15b-6a498bcbb05e.png align="center")

**Cloning**\- It will copy the remote repo to your local system.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1678092233342/26c04b43-5b41-474b-b02a-6b16752e80be.png align="center")

```bash
git clone <url of the repo>
```

This command will download the repo to your local system.

**Changes**\- Once downloaded you can use different code editors to change the files and make several changes that you want.

It is recommended that all the changes must be made in a new branch and not in the master branch so that our code does not break. We can do the same by the steps previously discussed.

**Pushing it into forked repo**\-After successfully committing our changes we need to push it into our forked repo. We can do the same by using the command:

```bash
git push origin <branch name>
```

**Creating pull request**\- After successfully pushing the changes to our forked repo we need to send a pull request to the owner of the original repo. If they merge it with their repo, hurray we made a contribution.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1678093254653/77c4ca92-f0eb-4042-8683-69fb32423cf4.png align="center")

### How to be in sync with the original repo?

Imagine you forked a repo on 12th Jan, and worked on it till 14th before submitting any pull request, there is a high chance that someone merged a pull request in between this time and your repo is outdated. To tackle this problem one needs to be in sync with the original repository, to do the same we use the following commands:

```bash
git remote add upstream <link of the original repo>
```

This command will add the upstream repo from where we can download the changes.

```bash
git fetch
```

The command git fetch will help us to download the changes.

```bash
git rebase
```

The command git rebase will add changes to my existing repo, and congo ur repo is updated.

### Conclusion

In conclusion git and github are powerful tools that every developer should learn to use effectively. By mastering these basics and following best practices you can collaborate with others easily and contribute to the open-source community.