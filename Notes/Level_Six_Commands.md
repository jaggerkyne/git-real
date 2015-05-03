# Senario:

Greg and Jane work on same file call 'readme.txt' at the same time.

Jane edited and pushed 'readme.txt' before Greg.

Greg useed 'git push' and returned an error.

Greg can use 'git pull' and 'git push' to merge the changes made by Jane to resolve this issue.
However, this method will polute the logbook on git.
We could use 'rebase' instead.

Greg can use 'git fetch' to get changes made by Jane on github but doesn't merge them with his own changes.
The Greg use 'git rebase' to:

1. Move all changes to master which are not in origin/master (changes made by Jane) to a temporary area.
2. Run all origin/master commits.
3. Run all commits in the temporary area, one at a time.
Note: There are no merge commit on the above steps using 'git rebase'.