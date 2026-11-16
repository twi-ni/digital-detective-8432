# Mission 6 - Git and GitHub

## Task 6.1 - Understand the Basic Git Workflow

In this task, I learned about the basic Git operations and how they help keep track of changes in a project.

### Git operations

| Git operation | What it does |
|---|---|
| Check repository status | Shows which files have been changed or are ready to be committed. |
| Stage selected changes | Selects the changes I want to include in a commit. |
| Create a commit | Saves the staged changes in the repository. |
| View commit history | Shows the commits made earlier in the project. |

### Difference between staging and committing

Staging means selecting the changes I want to save. Committing means saving those selected changes as a checkpoint in Git.

## Task 6.2 - Create and Use a Branch

I created a new branch called `update-about`. A branch lets me make changes separately without directly changing the main branch.
I then opened the root README file and added a section called My Learning.

After saving the changes, I checked the repository status, staged the README, committed the changes and pushed the branch to GitHub.

### 1. Create a new branch
Command used:
git switch -c update-about
This command created a new branch named `update-about` and switched me to it.
### 2. Check the current branch
Command used:
git branch
This command displayed the available local branches. The asterisk showed that I was currently working on `update-about`.
### 3. Check and stage the changes
Commands used:
git status
git add README.md
git status
I used `git status` to check which file had changed. Then I used `git add README.md` to stage the changes so they could be included in a commit.
### 4. Commit the changes
Command used:
git commit -m "Add my learning section to README"
This saved my changes in the Git history with a message explaining what I had added.
### 5. Publish the branch
Command used:
git push -u origin update-about
This uploaded my new branch to GitHub. Publishing the branch makes it available online and allows me to create a Pull Request from it.

## Task 6.3 - Create a Pull Request

After pushing my branch to GitHub, I created a Pull Request from `update-about` into `main`.
Pull Request title: Add My Learning section to README

A Pull Request is a way to suggest changes from one branch to another. It allows the changes to be reviewed before they are added to the main branch.
Branches and Pull Requests are useful because they allow people to work on separate changes and review them before combining their work.

**Pull Request status:** Open

## Task 6.4 – Build Your Git Command Glossary

In this task, I made a small glossary of the Git commands I learned while completing this mission. These commands help me manage my project, track changes and work with GitHub.

| Git operation | Command | What it does |
|---|---|---|
| Initialise a repository | `git init` | Creates a new Git repository in the current folder. |
| Check status | `git status` | Shows which files have been changed, staged or are untracked. |
| Stage changes | `git add` | Selects the changes that I want to include in my next commit. |
| Commit changes | `git commit` | Saves the staged changes in the repository's history with a message. |
| View history | `git log` | Shows the previous commits made in the repository. |
| Create or list branches | `git branch` | Creates a new branch or displays the available branches. |
| Switch branches | `git switch` | Changes from the current branch to another branch. |
| Publish changes | `git push` | Uploads my local commits to the remote GitHub repository. |
| Retrieve remote changes | `git pull` | Downloads and integrates the latest changes from the remote repository into my current branch. |

## What I Learned

I learned how Git keeps track of changes in a project. I also understood the difference between staging and committing, how branches work and how Pull Requests help people collaborate on projects.