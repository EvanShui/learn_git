# learn_git
## Repo
the purpose of this repo is to serve as a platform for me to learn how to use git and all of its functionalities. 
How to create repo via cmd line: 

'''
git init
'''

## Branches
The purpose of master is to hold the original code and the purpose of branches is to let other users experiment and make changes to
the original file without actually editting or making changes to the original file. Think of branches as a copy and paste of the master
branch. When users edit them, they aren't directly editting the master branch but instead, they are editting the copied branch. 
How to create a new branch via cmd line: 
`git checkout branch_name`
The same is used to switch between branches as well. For example if I were on a sub_branch and I wanted to switch to a master branch, I'd type out 
`git checkout master` 
to swtich to the master branch. 
If you added files to a sub_branch and you switched to the master branch, on your local repository, all of the changes you made, such as file creation, would also be reflected in the other branhces at that moment. To prevent that, you would have to push the new branch to the git repo with
`git push origin branch_name`
where branch_name is just the name of the new branch you created and after that, all of the changes you made on branch_name will only appear when you view branch_name and if you switch to another branch, such as master, the changes will dissapear. 
