# Merge a branch from another repository to the current branch
```
cd path/to/project-b
git remote add project-a path/to/project-a
git fetch project-a
git merge project-a/master # or whichever branch you want to merge
git remote remove project-a
```
from http://stackoverflow.com/a/10548919