# Git Assignment - To build a branching model


# Assignment Description

## Step-1: 
- First I created a empty folder in my local Computer and initialised an Empty repository.
- Now, I created a repository in remote environment named 'Git-Assignment' and linked my local repository with remote repository and pulled the readme.md file to local environment.

## Step-2:
- Now, In my local repository staying in my master branch(production branch) created two branched 'HotFix', 'Integration' using command
` git branch HotFix `
` git branch Integration `
- Now, I checked out to Integration branch using `git checkout Integration` command created other 2 branches `git branch feature1` and `git checkout feature2` commands
- After, I pushed all the changes from local to remote repository using `git push --all` command to reflect changes of all the branched created in remote repository.

## Step-3:
- Now, I checkeout to **feature2** branch and created a new file, now this file is currently in unstaged area of my local repository. To stage all the changes, I used `git add .` to add all the files. After staging all files, commit the changes using `git commit -m 'commit message'` command
- Now push the changes from **feature2** branch of local repository into remote repository using `git push origin feature2` command.
- After pushing feature2 branch into github, created a pull request to merge **feature2** into **Integration** branch by add two reviewers.
- Added a file in Feature2 and merged into Integration branch by creating the pull requests and adding reviewers requesting to merge.
- Now I deleted feature2 branch using `git branch -d feaature2` command, but using this command local branch is deleted. To delete remote branch also, I used `git push origin :feature2` command.

## step-4:
- In next step, Added a file in feature1 branch commited the changes in Local repository. Now I rebased my feature1 branch into Integration branch using `git rebase` command, so that all my local commits stay ahead of my remote changes.
- Now, Integration branch has all the changes from both feature1 branch and feature2 branch. I pushed all local changes of integration branch into remote using `git push origin Integration` command

# step-5:
- Now, I merged Integration into both Hotfix and master branches by using `git merge` command 
- Now to reflect these changes into remote repository, I pushed the changes of HotFix and Master branches using `git push origin Hotfix` and `git push origin master` commands.

# step-6:
- In this step, I checked out to feature1 branch and made change and committed into local environment.
- I pushed this changes into Github and created three pull requests by adding two reviewers to merge feature1 into Integration, Hotfix and master branches.
- After this, I got my PRs reviewed and merged feature1 into above mentioned branches.
- Now I deleted feature1 branch using `git branch -d feaature1` command, but using this command local branch is deleted. To delete remote branch also, I used `git push origin :feature1` command.

# step-7: 
- In this step, I made some changes in Hotfix branch and committed those changes in local repository. To push changes, I used `git push origin HotFix` command.
- To merge Hotfix into Integration and master branch, I created two pull requests to both branches by adding two reviewers.
- I got PRs reviewed and finally pulled those changes into local repository using `git pull origin Integration` and `git pull origin master` commands.

# Graph For Commit history

<img width="689" alt="Screenshot 2023-01-25 at 12 13 11 PM" src="https://user-images.githubusercontent.com/122455311/214500078-6c58f735-0dd0-4f0a-ba48-3674fa1b5338.png">


## Commands Used

`git init`

`git branch <branch name>`

`git checkout <branch name>`

`git add <file name>`

`git commit -m "commit message"`

`git push <remote> <branch>`

`git pull <remote> <branch>`

`git pull --rebase`

`git merge <branch name>`

`git branch -d <branch name>`

`git push origin :<deleted branch>`


