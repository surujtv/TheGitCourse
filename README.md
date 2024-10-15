
# what is git?
Git is a DevOps tool (software) used for source code management. It is a free and open-source version control system used to handle small to very large projects efficiently. Git is used to tracking changes in the source code, enabling multiple developers to work together on non-linear development.

# checking git version --> git --version
# use git bash terminal for windows

# Configuration Git - Set configs
# setting git configuration means we are telling git that In which account we are changing something.


# two type config -
1. global config (if we have single gitHub account)
2. local config


# setting global config
- git config --global user.name "your_github_user_name"
- git config --global user.email "your_github_email"
- git config --list 
  

# git commands -

# clone repositories from any gitHub account

- git clone gitHub_code_HTTPS_link

# check list of files inside directory
- ls

# check list of Hidden files inside directory
- ls -Hidden

# Check git status
- git status

# we have 4 type of status
1. modified - something changed inside existing files
2. untracked - added new file that git doesn't yet track
3. staged - file is ready to be committed
4. unmodified - unchanged

# Now Add code (adds new or changed files in your working directory to the git staging area0)
- git add . (add all files)
- git add file_name (add single file)

# Commit code (It is the record of change on our local machine in git)
- git commit -m "some message"

-------------------------------

# a new project, we need to initialize a new git repository -

- git init
- git add .
- git commit -m "initial commit"
- git remote add origin gitHub_code_HTTPS_link
- git remote -v (to check remote origin)
- git branch (to check current branch)
- git branch -M branch_name (to rename branch)
- git push origin main | git push -u origin main


# Git work flow
1. Create a gitHub Repo
2. Clone gitHub repo
3. Make changes
4. git add .
5. git commit -m "some message"
6. git push origin main


-------------------------------

# Git Branches -

1. git branch (check current branch)
2. git branch -M main (Rename branch)
3. git checkout -b new_branch_name (create new branch)
4. git checkout branch_name (to navigate another branch)
5. git branch -d branch_name (delete)

# NOTE: we can't delete existing branch.


# Merge git branches -

1. Way-1
   git diff branch_name (to compare commits, branches, files & more)
   git merge branch_name (to merge)

2. Way-2
   Create PR (Pull Request)

# What is pull request -
A pull request is a request to merge a branch into another branch on GitHub. It is a way to propose changes to a project without directly committing them.

It let's you tell others about changes you've pushed to a branch in a repository on GitHub.

-------------------------------

# Fetch remote changes on our local machine using pull command -
- git pull origin main (to fetch and merge changes)

# Pull command
used to fetch and download content from a remote repo and immediately update the local rep to match that content.

-------------------------------

# Git merge conflicts -
An event that takes place when Git is unable to automatically resolve differences in code between two commits at the same place.

# Resolving merge conflicts -
Manually by edit code.

-------------------------------

# Undoing changes - 

Case 1 - staged changes (git add .)
1. git reset file_name
2. git reset (all files)

Case 2 - committed changes (for one commit) 
1. git reset HEAD~1
2. git reset HEAD~n (for n commits)

Case 3 - committed changes (for many commits)
1. git reset commit_hash_value
2. git reset --hard commit_hash_value


# check all commits - 
- git log

-------------------------------

# Fork
A rough copy of a repository on GitHub. It is a way to create a new repository that is a copy of an existing repository.