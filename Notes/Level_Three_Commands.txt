# Cloning from repo, like github
git clone <URL of the remote repository>

# Example:
git clone https://github.com/codeschool/git-real.git

# If you want to clone a folder from the repository, you can use:
git clone <URL of the remote repository> <target folder>

# Example:
git clone https://github.com/codeschool/git-real.git git-demo

# What does clone do?

# 1. Downloads the entire repository into a new git-real directory.
# 2. Adds the 'origin' remote, pointing it to the clone URL
# You can run below command to see
git remote -v

# 3. Checks out initial branch (likely master). -- sets the head.

# After clone the existing code, we need to branch out before working on new feature
# Create branch from master
git branch <branch name>

# E.g.
git branch cat

# Use this command to see:
git branch

# Time to jump on new branch
git checkout <branch name>

# E.g.:
git checkout cat

# Then work on new feature on cat timeline
# After finishing new feature, we need to switch back to master branch
git checkout master

# Merge new feature with master, using:
# merge brings one branch's changes into another.
git merge cat

# When you're done with a branch, you can safely remove it.
git branch -d <branch name>
# E.g.
git branch -d cat

# A fast way to create and switch to the branch
git checkout -b <branch name>

# E.g.:
# Create a branch call admin and check it out.
git checkout -b admin

# Time to put out the fire.
# We'll back to that admin branch later.

# Move to master branch
git checkout master

# Check we are indeed on master
git branch

# Make sure we have the lastest code by pulling code on repo
git pull

# put out fires:

git add store.rb
git commit -m 'Fix store bug'

git add product.rb
git commit -m 'Fix product'

# push to code to remote repo after putting out fire.
git push

# Now it's time to move back to work on admin feature
git checkout admin

# Work on admin feature

# time to meger new feature with master

git checkout master

# Merge the admin feature with master
git merge admin

# Now we are at vi editor

# Vi commands:

# J down K up
# H left l right
# ESC leave mode
# i insert mode
# :wq save & quit
# :q! cancel & quit





