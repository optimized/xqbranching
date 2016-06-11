# Exquisite Branching Model

## Resources
https://guides.github.com/introduction/flow/
https://skoch.github.io/Git-Workflow/

## Branching with git

There are three branches: master, staging, and production

### Create a branch from master called myfeature
``git checkout -b myfeature master``

### check out master and merge to staging
```
git checkout staging
git merge --no-ff master
git push origin staging
```

### check out staging and merge to production
```
git checkout production
git merge --no-ff staging
git push origin production
```

### Developing in your own branch
```
git checkout -b myfeature master
git checkout master
git merge --no-ff myfeature
git branch -d myfeature
git push origin master
```
