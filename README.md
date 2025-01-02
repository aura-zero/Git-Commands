# Git Commands

## Configration email and user name

### Global
```zsh
git config --global user.email "you@example.com"
git config --global user.name "Your Name"
```
### Local
```zsh
git config --local user.email "you@example.com"
git config --local user.name "Your Name"
```
### Unset
```zsh
git config --global --unset user.email
git config --global --unset user.name
```

## Getting Started with new repo

```zsh
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/[username]/[repo-name].git
git push -u origin main
```

## Post Configration and Setup 
```zsh
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




## forkeeed

```zsh
git clone --bare <https://github.com/exampleuser/public-repo.git>
cd public-repo.git
git push --mirror <https://github.com/yourname/private-repo.git>
```

## Working with submodules
Eventually, any interesting software project will come to depend on another project, library, or framework. Git provides submodules to help with this. Submodules allow you to include or embed one…

You can add "sub_repo" as a submodule of main. In the main repository:
```zsh
git submodule add https://github.com/<user>/sub_repo part_of_main_now
```

Newer versions of Git will do this automatically, but older versions will require you to explicitly tell Git to download the contents of sub_repo:

```zsh
git submodule update --init --recursive
```

Joining a project using submodules
```zsh
git clone --recursive <main repo url>
```
