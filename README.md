# Git Workflow

## Setup and Initiation

- `git config --global user.email "you@example.com"`
- `git config --global user.name "Your Name"`

```git
git config --local user.email "you@example.com"
git config --local user.name "Your Name"
```

## Unset

```git
git config --global --unset user.email
git config --global --unset user.name
```

- ### New Repository

  - `git init`
  - `git add README.md`
  - `git commit -m "first commit"`
  - `git branch -M main`
  - `git remote add origin https://github.com/[username]/[repo-name].git`
  - `git push -u origin main`

## Post Configration worlflow

1. `git add .`
2. `git commit -m "something has changed"`
3. `git push origin main`
4. `git pull origin main`

## Getting Started and Testing
>
> Check your login details

- `git config --list`

> Check Status or State of your repo

- `git status`

> List Branches | `-a` denotes all Branches

- `git branches`

> View Changes You and Other made | `--oneline` denotes all commit id and name (no details)

- `git log`

> Remove a file

- `git rm -r [file-name.git]`

## Branching and Merging
>list your branches. a * will appear next to the currently active branch

git branch
>create a new branch at the current commit

git branch `branch-name`
>switch to another branch and check it out into your working directory

git checkout `Branch-Name`
>merge the specified branch’s history into the current one

git merge `branch_name`
>show all commits in the current branch’s history

git log


## How to make frolked repo private

```git
git clone --bare <https://github.com/exampleuser/public-repo.git>
cd public-repo.git
git push --mirror <https://github.com/yourname/private-repo.git>
```
