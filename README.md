# Git Assignment - To build a branching model

<img width="689" alt="Screenshot 2023-01-25 at 12 13 11 PM" src="https://user-images.githubusercontent.com/122455311/214500078-6c58f735-0dd0-4f0a-ba48-3674fa1b5338.png">



Above picture represents the commit history of this repopsitory.

- It contains 5 Branches - Production (master), Integration, HotFix, Feature1, Feature2

- First created a git repository locally and created Production(master), Integration and HotFix branch. And after created other two branches Feature1 and Feature2 from Integration Branch. 

- Added some files in Feature2 and Feature1 are merged into Integration branch by creating the pull requests and adding reviewers requesting to merge.

- In next step, changes in Integration branch merged into Production(master) and HotFix branch

- Now, In HotFix branch made a quick fix and merged into Integration and Production branch

- Finally deleted Feature1, Feature2, HotFix branches after completing the above steps.

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


