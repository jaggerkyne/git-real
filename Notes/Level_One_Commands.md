Git is a Distributed Version Control System aka DVCS.

# Command to get help
git help

eg: git help config

# Initial Settings after installing Git

# Setting user name
git config --global user.name "Jagger Kyne"

# Setting user email
git config --global user.email jagger.kyne@gmail.com

# Enable color scheme
git config --global color.ui true


# Starting a Repo

mkdir store

cd store

# initialized empty Git repository in /Users/username/store/.git/

git init

# Git Work Flow

Jane Creates Readme.txt file -- starts as untracked

Add file to staging area -- getting ready to take a picture

Commit changes -- A naptshot of those on the stage

Jane modified Readme.txt file & adds License

Add both files to staging area

Commit changes

# To check what's changed since last commit

git status

# Add the list of files
git add <list of files>

# Add Readme.txt to stage e.g.:
git add Readme.txt

git commit -m "Create a Readme"

# Adds all new or modified files.
git add --all

# View the commit history
git log

# Add all txt files in current directory
git add *.txt 

# Add all txt files in docs directory
git add docs/*.txt

# Add all files in docs directory
git add docs/


# Add all text files in the whole project
git add "*.txt"


