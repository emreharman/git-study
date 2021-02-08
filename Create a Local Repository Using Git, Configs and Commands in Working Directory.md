## Create a Local Repository Using Git, Configs and Commands in Working Directory

- At first you must setup git. You can download and setup it [from there](https://git-scm.com/download) choosing your operating system.
- Then check if it's ok writing console `git --version`. If you see something like `git version 2.30.0.windows.2`, now you can start using Git.

- Now create a folder you want to build a project or open an existing folder. Then click right and select **Git Bash Here**. Command `git init`. That's all. Our local repo is created. After that Git will realise all changes but will do nothing untill you command it put them to the staging area.

- Let's make some changes in this folder. Create a file anything you want (test.txt, index.html ...). Now command `git status`. This command shows your repo's status. Let me explain this command shortly. It tells us about which branc we're on, changed files or added files which not put to the staging area as **Untracked Files** and the files on the staging area waiting to commit. We will use this command a lot to know about our repo's status.

- We've made changes on our repo and seen it's status as untracked files. now command `git add yourFileName`. This command puts your file to the staging area. If you have more than one file as untracked files and you want to put all of them to the staging area, use `git add .` command. Now our changes are at the staging area.

- Let's talk about Git configs. Use `git config --list` command. This command lists your git configs. The most important config that we use is **user.name** and **user.email**. Git uses these configs in the commits as a signature. To set these configs we use `git config --global user.name yourUserName` and `git config --global user.email yourEmail`. The global parameter sets them in global. If you don't use this parameter it sets just in current git repo.
