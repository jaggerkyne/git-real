# Why create a remote branch?
# When you need other people to work on your branch.
# Any branch that will last more than a day.

# Create a shoppingcart remote branch

# Create a branch call shopping_cart and switch to it
git checkout -b shopping_cart

# Push branch shopping_cart to remote repo
# Links local branch to the remote branch and start tracking it.
git push orgin shopping_cart

# Jane Pulling new branches
git branch

# List all remote branches.
git branch -r

# Branch shopping_cart set up to track remote branch shopping cart from origin. Swithed to a new branch "shopping_cart"
git checkout shopping_cart

git remote show origin

# Delete a remote branch
git push origin ：shopping_cart

# Delete the respective local branch
git branch -d shopping_cart

# Delete the respective local branch
git branch -D shopping_cart

# No remote to push to (It's just a local branch now)
git remote show origin

# To clean up deleted remote branches
# prune branches every once for a while. 
git remote prune origin

# Heroku deploys only master branch

$ git branch
 * staging
   master

# Would not work, would push to staging
$ git push heroku-staging staging

# Will push and deploy staging on heroku
# staging is our local branch
# master is heroku branch
$ git push heroku-staging staging:master

# A tag is a reference to a commit (used mostly for release versioning)

# list all tags
git tag

# make a tag
git tag v0.0.1

# check out code at commit
git checkout v0.0.1

# push tags to remote repo
git push --tags

# Delte a remote tag
# http://stackoverflow.com/questions/5480258/how-to-delete-a-remote-git-tag
git push origin :<tag_name>








