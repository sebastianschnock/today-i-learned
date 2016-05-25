# Reset your branch from a forked repo to the state of the upstream version

```
# add upstream
git add remote upstream <url>
# get latest upstream
git fetch upstream
# switch to the branch to be reset
git checkout <branch>
# get state from upstream
git reset --hard upstream/<branch>
# push it through
git push -f origin <branch>
```