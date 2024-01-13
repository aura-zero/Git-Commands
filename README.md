# Git Commands

## Configration email and user name

### Global
```git
git config --global user.email "you@example.com"
git config --global user.name "Your Name"
```
### Local
```git
git config --local user.email "you@example.com"
git config --local user.name "Your Name"
```
### Unset
```git
git config --global --unset user.email
git config --global --unset user.name
```

## Getting Started with new repo

```git
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/[username]/[repo-name].git
git push -u origin main
```

## Post Configration and Setup 
```
git add .
git commit -m "something has changed"
git push origin main
git pull origin main
```
## Check Status and Inspect
|Discription | Command |
|----|----|
|Check your login details|git config --list|
|Check Status or State of your repo|git status|
|List Branches `-a` denotes all Branches|git branches|
|logs ,`--oneline` denotes all commit without extras|git log|




## Branching and Merging
|Discription|Commands|
|----|-----|
|list your branches. a * will appear next to the currently active branch|git branch|
|create a new branch|git branch `branch-name`|
|switch to another branch and check it out into your working directory|git checkout `Branch-Name`|
|merge the specified branch’s history into the current one|git merge `branch_name`|





## How to make frolked repo private

```git
git clone --bare <https://github.com/exampleuser/public-repo.git>
cd public-repo.git
git push --mirror <https://github.com/yourname/private-repo.git>
```
