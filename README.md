# Git Workflow

## Setup and Initiation
- `git config --global user.email "you@example.com"`
- `git config --global user.name "Your Name"`

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
> Check Status or State of your repo
- `git status`
> List Branches | `-a` denotes all Branches
- `git branches ` 
> View Changes You and Other made | `--oneline` denotes all commit id and name (no details)
- `git log `
> Remove a file
- git rm -r [file-name.git]

## Branching and Merging
.... will be added later.