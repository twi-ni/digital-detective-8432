# Mission 6 – Git and GitHub

## 1. Task 

The aim of this mission was to understand how Git and GitHub work and how they help us manage changes in a project. I practised checking repository status, staging and committing files, creating a branch and opening a Pull Request.

## 2. Work Completed

### Task 6.1 – Basic Git Workflow
- Checked the status of my repository using `git status`.
- Made a small change to the root README file.
- Staged the file using `git add`.
- Created a commit with a meaningful message.
- Checked the recent commit history using `git log`.

### Task 6.2 – Create and Use a Branch
- Created a new branch called `update-about`.
- Added a section called "My Learning" to the root README.
- Checked and staged the changes.
- Committed the changes and pushed the branch to GitHub.

### Task 6.3 – Create a Pull Request
- Opened my repository on GitHub.
- Created Pull Request #1 from `update-about` into `main`.
- Added a title and description explaining the README changes.
- Checked the Pull Request details on GitHub.
- Left the Pull Request open without merging it, as I was not instructed to merge it.

### Task 6.4 – Git Command Glossary
- Prepared a glossary of important Git commands.
- Added explanations for commands used to check status, stage changes, commit, view history, manage branches and exchange changes with GitHub.

## 3. Commands and Tools Used

| Command | Purpose |
|---|---|
| `git status` | Checks the current state of the repository. |
| `git add README.md` | Stages the README file. |
| `git commit -m "message"` | Saves staged changes with a commit message. |
| `git log -5 --oneline` | Displays recent commits. |
| `git switch -c update-about` | Creates and switches to a new branch. |
| `git branch` | Lists available branches. |
| `git push -u origin update-about` | Publishes the branch to GitHub. |
| `git switch main` | Switches back to the main branch. |
| `git pull` | Retrieves and integrates remote changes. |

**Other tools used:** Terminal, VS Code and GitHub.

## 4. What I Understood

I understood that Git helps track changes made to files and keeps a history of the work.
I also learned that staging and committing are not the same thing. Staging selects the changes that I want to save, while committing actually records those changes in Git history.
A branch allows me to work on changes separately without directly modifying the main branch. A Pull Request is used to propose those changes for review before merging them into the main branch.
I also understood how `git push` and `git pull` help keep my local project and the GitHub repository updated.

## 5. Difficulties Faced and How I Solved Them

While working on this mission, I noticed that some `.DS_Store` files were appearing in my Git status. These are macOS metadata files and were not needed in my repository.

To solve this, I created a `.gitignore` file in the root folder and added `.DS_Store` to it. This stopped Git from showing those files as untracked changes.
I also learned how to work with branches and Pull Requests through the GitHub interface.

## 6. Evidence and Files

Screenshots of the commands and pull request.