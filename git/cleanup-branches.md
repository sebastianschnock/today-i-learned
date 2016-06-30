# clean up local branches (exclude master and development)
```
git branch --merged | grep -v "\*" | grep -v master | grep -v development | xargs -n 1 git branch -d
```

# clean up remote branches (on origin, exclude master and development)
```
git branch -r --merged master | grep -v master | grep -v development | cut -d/ -f2- | xargs -n 1 git push --delete origin
```