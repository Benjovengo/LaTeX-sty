LaTeX .sty Package for Lectures
=

benjovengo.sty package for my lectures.

Introduction
===

Each individual lecture will cover one day of class and is treated as a chapter (with mini table of contents).


Git Commands
===

Stage and Commit in one command
```git commit -am "commit message"```

and 

```git push```

Stage before a commit (to commit separate parts)



You can use SmartGit for a GUI for git on Linux: http://www.syntevo.com/smartgit/index.html

But learning git first on the command line is generally a good idea:

Below are some basic examples assuming you are only working from the master branch:

Example for starting a local repo based on what you have from github:

```git clone https://github.com/sampson-chen/sack.git```

To see the status of the repo, do:

```git status```

Example for syncing your local repo to more recent changes on github:

```git pull```

Example for adding new or modified files to a "stage" for commit

```git add /path/file1 /path/file2```

Think of the stage as the files that you explicitly tell git to keep track of for revision control. git will see the all the files in the repo (and changes to tracked files), but it will only do work on the files that you add to a stage to be committed.

Example for committing the files in your "stage"

```git commit```

Example for pushing your local repo (whatever you have committed to your local repo) to github

```git push```

Caching your GitHub password in Git
===

If you're cloning GitHub repositories using HTTPS, you can use a credential helper to tell Git to remember your GitHub username and password every time it talks to GitHub.

If you clone GitHub repositories using SSH, then you authenticate using SSH keys instead of a username and password. For help setting up an SSH connection, see Generating an SSH Key.

Tip: You need Git 1.7.10 or newer to use the credential helper.

Turn on the credential helper so that Git will save your password in memory for some time. By default, Git will cache your password for 15 minutes.

    In Terminal, enter the following:

    ```$ git config --global credential.helper cache```
    # Set git to use the credential memory cache

    To change the default password cache timeout, enter the following:

    ```$ git config --global credential.helper 'cache --timeout=3600'```
    # Set the cache to timeout after 1 hour (setting is in seconds)


