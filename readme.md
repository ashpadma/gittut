Hello World!

# Git Commands

## Basic

    git
    git init        - To create and initialize a git repo
    git status      - To see the status of git folder or repo
    code <filename> - To create a file using VScode (then manually save it)
    git add <filename>  - To add file to git for tracking
    git add .           - To add all new files
    git commit -m "<comment>" - To commit changes into the folder or repo

## Connect local to remote in Git using SSH
    ssh-keygen -t rsa -b 4096 -C "<email>" - To generate a key
    eval $(ssh-agent -s)        - To check status of ssh running
    ssh-add ~/.ssh/id_rsa       - To add generated key to ssh

        Then go to "C:/Users/<user>/.ssh" and open id_rsa with notepad
        and copy the whole text. Paste it on Github ssh key section for
        new key and give it a name. 

    ssh -T git@github.com       - To verify and next steps (type: yes)


## Repo commands
    git clone <"url">
    git push origin main    - To push committed new files to repo in Github
    git fetch               - To fetch the repo from Github to local(if there are changes)
    git pull                - To reflect the fetched changes into the local repo
    
## Branching and Forking
    git branch <branch name>    - Create a local branch
    git checkout <branch name>  - Switch to the local branch
    git checkout -b <'branch name'> - Make new branch and switch to in one command
    git push -u <origin> <branch>   - Push changes in local branch to main branch