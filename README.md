# Git and GitHub
- Git is a version control system
- GitHub is a place for hosting Git-based projects

## References
- [Git website docs](https://git-scm.com/doc)

## Steps
- git init

Create files and stage them (Add to staging area and make them ready for a commit)
- git add .

Commit them
- git commit -m "First cut - blah blah"

To check staged files
- git status

To check history of commits (on current branch)
- git log 

To create a branch
- git branch <branch_name>

To shift a branch
- git checkout <branch_name>

To rename a branch
- git branch -m <old_branch_name> <new_branch_name>

To merge from another branch
Shift to the branch into which you want to bring the commits from another branch (eg. we checkout main / master)
- git merge <other_branch_name>
You may get merge conflicts in multiple files (potentially) - resolve them, test the file, and then commit.

## Working with GitHub
Create a GitHub repo (login and create a new repo). Follow the steps shown after creating repo (skip the steps that create the local git repo and commit)
- git remote add origin <origin_url>
- git push -u origin <branch_to_push_to_on_remote>
_NOTE_: branch_to_push_to_on_remote is usually same as the current local branch name (eg. main / master / ...etc.)