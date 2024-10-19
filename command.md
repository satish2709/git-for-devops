
# Git Commands

# Create a directory and initialize a Git repository
mkdir git-for-devops
cd git-for-devops/
git init

# Create files and check their status
touch hello-dosto.txt
touch nibba.txt nibi.txt
git status

# Add files to the staging area
git add nibba.txt
git status
git add nibi.txt
git status

# Commit the added files
git config --global user.name "satish2709"
git config --global user.email "sardake27@gmail.com"
git commit -m "add nibba" nibba.txt
git status
git commit -m "add nibi" nibi.txt
git status

# Remove a file and restore it
rm nibi.txt
git status
git restore nibi.txt
git status

# Check Git log and make changes to a file
git log
vim nibba.txt
git add nibba.txt
git commit -m "new changes to nibba"
git log

# Create a new branch and work with it
git checkout -b dev
git branch
touch nibbu.txt
git add nibbu.txt

# Switch between branches and commit changes
git checkout master
git status
git commit -m "added nibbu" nibbu.txt
git branch
git checkout dev
git branch
git log
git checkout master
git log

