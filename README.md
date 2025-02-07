# GitHub Commands Guide

## Creating and Navigating Directories
sh
mkdir project
cd project
mkdir src
cd src
touch a.txt


## Writing to a File
sh
echo "hello this is my first file" >> a.txt

## Adding multiple line text to file
sh
echo -e "hello this is my first file\n I'm writing to the file" >> a.txt && cat a.txt # to display file content in console

## Viewing Git Commit History
sh
git log  # Show the commit history with details

## Resetting to a Specific Commit (Soft Reset)
sh
git reset --soft cf448  # Move HEAD to a specific commit without changing working files


## Creating and Committing a New File
sh
echo 'b' > b  # Create a file 'b' and add content
git add b  # Stage the file for commit
git commit -m "b"  # Commit the staged file with a message

## Creating and Managing Branches
sh
git branch featureb  # Create a new branch named 'featureb'


## Listing All Branches
sh
git branch  # Display all branches in the repository

## Switching to a Branch
sh
git checkout featureb  # Switch to the 'featureb' branch

## Viewing Commit History in One Line
sh
git log --oneline  # Show commit history in a condensed format


## Rebasing onto Main Branch
sh
git rebase main  # Reapply commits on top of the 'main' branch

## Creating a new Branch 
sh
git branch -C featureb featurec  # copy 'featureb' to 'featurec'


## Merging a Branch into the Current Branch
sh
git merge featureb  # Merge 'featureb' into the current branch


## Squashing Commits Before Merging
sh
git merge featureb --squash  # Combine all commits from 'featureb' before merging
