Level 4 Notes on master.

# When two or more people working on the same project,

# they may commit changes simutansouly and push to the remote repo.

# We need to pull the lastest changes from the remote repo before push our changes to the remote repo, like:

# 1. Fetch (or sync) our local repo with the remote one
# 2. Merges the origin/master with master 
# ($ git fetch)
# ($ git merge origin/master)

git pull
# Update origin/master be at the same state as our local repo.
git push


# Working on same file and one push first than other.

# we need to manually fix that then commit.



