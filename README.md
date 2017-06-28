# learn_git
## Repo
the purpose of this repo is to serve as a platform for me to learn how to use git and all of its functionalities. 
How to create repo via cmd line: 

`
git init
`

## Branches
The purpose of master is to hold the original code and the purpose of branches is to let other users experiment and make changes to
the original file without actually editting or making changes to the original file. Think of branches as a copy and paste of the master
branch. When users edit them, they aren't directly editting the master branch but instead, they are editting the copied branch. 
How to create a new branch via cmd line: 

`git checkout branch_name`

The same is used to switch between branches as well:

`git checkout master
git checkout branch_name`

If you added files to a sub_branch and you switched to the master branch, on your local repository, all of the changes you made, such as file creation, would also be reflected in the other branhces at that moment. To prevent that, you would have to push the new branch to the git repo:

`git push origin branch_name`

Branch_name is just the name of the new branch you created and after that, all of the changes you made on branch_name will only appear when you are on branch_name. If you switch to another branch, such as master, the changes will dissapear. To view which branch you are on:

`git branch` 

## Adding / Commiting

Adding will stage your files for committing, your essentially telling git which files you want to get ready to push to your git repo, usually its the files you have editted: 

`
git add file_name
git add *
`

You can use the wildcard * to add all files.

Commiting is saving the changes you've made on whatever files you've editted / added. To stage your commit and to add a meaningful message behind what edits you've made:

`git commit -m "message"`

## Pull Request

So what is a pull request? A pull request is a request to essentially combine the current branch with another branch. Usually in a group setting, you could create a pull reqeust and ask other's for feedback. To pull files from a different repo to the branch you want to pull to:

`git checkout target_branch_you_want_to_pull_to
git pull origin target_branch_you_want_to_pull_to`

In a group setting, there are many advantages to this. For one, if someone creates a sub branch from the master, and wants to combine the edits they've made back to the master, they could use pull for this. Individually, this can also be helpful if you want to make edits to the master without actually editting the master. 

## Pushing 

After adding, commiting, or pulling files, the last step is to actually push the files to the git repo. All of the previous commands have been to edit the files locally, however in order to "finalize" the edits, you have to push them to the git repo: 

`git push origin branch_name` 

## Conclusion

And that pretty much sums up the most basic major functions of github. Of course there's a lot more than just this, however at my current state, this is all I need to know. 

 

