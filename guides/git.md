# Introduction to Git and GitHub

## What is Git?

Git is a distributed version control system created in 2005 to help developers track changes in their projects over time. It allows you to record modifications to files, revert to previous versions, and collaborate efficiently with other developers.

Git runs locally on your machine and works primarily through the terminal, although graphical interfaces are also available.

With Git, you can:

* Track changes in your code
* Create snapshots of your project using commits
* Work on different features using branches
* Merge changes from different branches
* Revert to previous versions when necessary

Example of basic Git commands:

```bash
git add .
git commit -m "Add new feature"
```

The `git add` command stages changes, and `git commit` saves a new version of the project in the repository history.

---

## What is GitHub?

GitHub is a cloud-based platform that hosts Git repositories online. It allows developers to store their projects remotely and collaborate with others.

While Git is the version control system itself, GitHub provides a web interface and additional tools to manage and share Git repositories.

With GitHub, you can:

* Store repositories in the cloud
* Collaborate with other developers
* Manage contributions through pull requests
* Track issues and bugs
* Share projects publicly or keep them private

---

## Git vs GitHub

It is important to understand the difference:

* **Git** is the tool that tracks and manages changes locally.
* **GitHub** is the platform that hosts Git repositories and enables collaboration.

In simple terms, Git controls versions of your project, and GitHub allows you to store and share those versions online.


<details>
    <summary>Read more</summary>

### Create / initialize Repository:
    git init - **INIT**ialize repository
    git clone URL (<link>) - clone a repository
git clone https://github.com/user/repository.git



### Check status and hirtory:
    git status - show current state
    git log - commit history
    git log --oneline -> compact history
    gi log --graph -> graphical history
    git diff - show changes



### Add files (Staging Area):
    git add <file name>
    git add . -> all files and posters
    git reset <filename> -> Remove from staging



### Commit:
    git commit -m "message"
    git commit -am "message"
    git commit --amend -> edit last commit



### Work with Remote (GitHub)
    git remote add origin <repository-link> -> add remote respository
    git remote -v -> view remotes
    git remote remove origin -> remove remote
    git push -u origin main - push to github
    git push - after 1st push
    git pull - pull changes
    git fetch - fetch without merging



### Branches:
    git branch <branch-name> -> create branch
    git branch - list branches
    git checkout <branch-name> -> switch branch
    git switch <branch-name>
    git checkout -b <branch-name> -> create and switch
    git switch -c <branch-name> -> create and switch
    git branch -d <branch-name> -> delete branch



### Merge:
    git merge <branch-name>



### Reset (⚠️):
    git reset --soft HEAD~1 - Undo last commit but keep changes
    git reset -- hard HEAD~1 - Delete commit and changes completely



### Revert:
    git revert COMMIT_HASH - Undo a commit by creating a new commit



### Tags:
    git tag v1.0 - Create tag
    git push origin v1.0 - push tag
    git tag - list tags



### Remove files:
    git rm file - remove file from git
    git rm -cached file - remove from git but keep locally



### Stash (Temporary Save):
    git stash - save changes temporarily
    git stash list - list stashes
    git stash pop - restore last stash



### Advanced History:
    git show COMMIT-HASH
    git blame <file>



### Remove Git completely:
    rm -rf .git



### Basic daily workflow:
    git add .
    git commit -m "message"
    git push



### List how to start:
    git init
    git add .
    git commit -m "initial commit"
    git branch -M main
    git remote add origin <repository-link>
    git push -u origin main -> first push



</details>