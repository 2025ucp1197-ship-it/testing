# Git and GitHub

Git keeps track of changes made to project files. GitHub hosts Git repositories online so that code can be shared and reviewed. They are related, but Git is the version control tool and GitHub is the hosting and collaboration platform.

## Main Git workflow

A repository stores the project history. Files start in the working directory, selected changes move to the staging area, and a commit records a snapshot in the local repository. A tracked file is one that Git is already managing; a new file is untracked until it is added.

- git init: start a repository in the current folder.
- git status: see modified, staged and untracked files.
- git add main.py: stage one file.
- git add .: stage changes from the current directory.
- git commit -m "Add calculator": record staged changes with a message.
- git log --oneline: view short commit history.
- git diff: inspect unstaged edits.
- git diff --staged: inspect staged edits.
- git restore --staged main.py: unstage a file without deleting its edits.
- git restore main.py: discard unstaged changes in a tracked file, so use carefully.
- git revert COMMIT_ID: make a new commit that reverses an earlier commit.

## GitHub and remote repositories

- git remote add origin URL: connect a local repository to a remote.
- git remote -v: check configured remotes.
- git push -u origin main: publish the main branch and set its upstream.
- git clone URL: make a local copy of a repository and its history.
- git fetch origin: download remote updates without merging them into the current branch.
- git pull origin main: fetch and integrate changes from the remote main branch.

## Branches and collaboration

A branch allows a new feature to be developed separately from main. git branch lists branches; git switch -c feature-login creates a branch and switches to it. git switch main returns to main, and git merge feature-login integrates that feature into the current branch. When changes clash, a merge conflict must be resolved manually.

On GitHub, a pull request proposes changes for review before merging. A fork is a separate hosted copy of someone else's repository, while clone creates a local copy. Issues are used to track tasks and bugs. Tags such as v1.0.0 can mark releases. A .gitignore file tells Git which untracked files, such as temporary logs, should normally be ignored.
