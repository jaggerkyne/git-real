Level Two Command

# Show unstaged differences since last commit
git diff

# After adding file on stage, we can view the differences using
git diff --staged

# Unstage a file after it is staged
# HEAD refers to last commit at current timeline.
git reset HEAD <file name>

# Blow away all changes since last commit
git checkout -- <file name>

# Don't Use them AFTER you push.
# undo last commit, put changes into staging.

# Add changes from all tracked files,
# All untraced files are not added.
git commit -a -m "Modify readme"

# Reset into staging, move to commit before "HEAD".
git reset --soft HEAD^ 

# Change the last commit
git commit --amend -m "New Message"

# Undo last commit and all changes
git reset --hard HEAD^

# Undo last 2 commits and all changes.
git reset --hard HEAD^^

####Working with Remotes
git remote add <our name for this remote> <Address>

# Example:
git remote add origin https://github.com/jaggerkyne/git-real.git


# View all the remote repos
git remote -v

# Push change to remote repo
# Note: "origin" is the remote repository name
# Note: "master" is the local branch to push 
git push -u origin master

# Password caching: https://help.github.com/articles/set-up-git


# To pull code from remote repo
git pull

# To add new remotes
git remote add <name> <address>

# To remove remotes
git remote rm <name>

# To push to remotes, please noted <branch> usually master
# "-u" below allows you to use "git push" later on after you run the code below.
git push -u <name> <branch>

# Heroku usage:

# Create Heroku project
heroku create

# View all the remote address
git remote -v

# triggers deploy
git push heroku master 