# Doumentation
Git  Documentation
===============
What is git? 

Git is powerful, sophisticated system for distributing version control.Gaining an understanding of its features open to developers a new and liberating approach to source code management.

Git as two repositories 1. Local repository
                                          2. Remote repository

The Local repository  is the one on which will be make local changes,typically this local repository is on own  machine. 

Git repository is the one of the server , typically a machine  situated at 42 miles aways.

How to install git ?
https://github.com/git-guides/install-git

Git commands:

Git init
=====
The git init command creates a new Git repository. It can be used to convert an existing,unversioned project to a Git repository or initialize a new empty repository.

Git add 
======
The git add command adds new or changed  files in your working directory to the git staging area. 
Git add is an important command -without  it , no git commit  would ever do anything.Sometimes, git add can have a reputation for being an unnecessary step in development. But in reality git add is an important and powerful tool.git add allows you to shape history without changing how you work.
git add <path> stage a specific directory or file

git add .  stage all files

Git reset 
=======
Git reset is a flexible and powerful command.one of its many use cases is to move changes out of the staging area. To do this, use the mixed level of reset 

To move staged changes from the staging area to the working directory without affecting committed history 

Git reset HEAD  asked  git reset –mixed HEAD .

Git clone 
=======

The git clone command is used to create a copy of specific repository or branch within a repository.
Git is distributed version control system.maximize  the advantages of a full repository on your own machine by cloning

Git clone https/ssh url
Git clone a branch 


When you  clone a repository you don”t get one file,like you many in other centralized version control systems by cloning with git you get the entire repository all files ,all branches, and all commits.

Git commit 
=========
Git commit creates a commit,which is like  a snapshot of your repository.these commits are snapshots of your entire repository at specific times.you should make new commits often,based around logical units of change.

Commits have two phases to help you craft commits properly.commits should be 	logical atomic units of change that represent a specific idea but not all humans work that way. You may get carried away and end up solving two or three problems before you remember to commit .

Once your ready to craft your commits,you’ ll use  git add <fill name>

How to use git commit
==================

Git commit -m “commit name” msg

What does git remote do?

Git remote manages the set of remotes that  you are tracking with your local repository
Git remote commands
=================

Git remote -v 

Git remote add [url]

Git remote remove [name]


What is origin
===========

If you try running git remote -v in your repositories you Ll probably see something called origin
You many notice origin in many messages from git origin in the human-friendly 
Name for url that the remote repository is stored at it s like a key value  pair and origin is the default 



What is upstream
=============

You many need or want  to work with multiple  remotes for one local repository.
This can be common in open source ,when a contributor needs to create a fork of a repository to have permission to push changes to the remote 



Git status 
========

Git status shows the current state of your git working directory and staging area

When in doubt run git status  this  always  a good idea. The git status command only outputs information it won’t modify commits or changes in your local repository

If changed files are staged or not 

If your current local branch is linked to a remote branch than git status will tell you if your local branch is behind or ahead by any commits

Git status 

Git status -v
 
Git status  -s


Git pull
============

Git pull updates your current local working branch,and all of  the remote tracking branches . its a good idea to run git pull regularly on the branches you are working on locally.

Without git pull  your local branch wouldn’t have any of the updates that are present on the remote 


Git pull is one of the 4 remote operations within git. Without running pull your local repository  will never be updated with changes form  the remote.

Git pull should used every day you interact with a repository with are remote at the minimum thats the git pull most important command


Git pull

Git pull –rebase 

Git pull –force

Git pull –all


Git push
================

Git push uploads all local branch commits to the corresponding remote branch 

Git push updates the remote branch with local commits. It is one of the four commands in git that prompts interaction with the remote repository

You can also think of git push as update or publish 

Git push -f 

Git push -u origin branch name

Git push –all

Git push –tags
Git cherry-pick 
===============

Git cherry-pick is a powerful command that enables arbitrary git  commits to be picked by reference and appended to the  current working head 
Cherry picking is the act of picking a commit from a branch and applying it to another 

Git cherry-pick can be useful for undoing changes

========================================





















