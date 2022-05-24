
    
# How to do it with just the command line
1. Create a new repository on GitHub and initialize it with a README file
2. Create a folder on your local machine
3. Open terminal and move to that folder
$ cd FOLDER
4. Add the remote URL as origin
$ git remote add origin https://github.com/USERNAME/REPOSITORY_NAME.git
5. Now using the pull command, you can ‘pull’ down the README file onto the local folder
a. $ git pull origin master
6. Add your current files in the local folder to the staging area
a. $ git add –-all
7. Commit your changes
$ git commit -m "your commit message e.g. First commit"
8. Push your changes to the master branch
$ git push origin master


# How to Create branch in git hub commond line

$ git status

# create new branch
$ git branch alpha

# list of branch
$ git branch --list
alpha

# list of all local and remote branch
$ git branch -a

- master

# swich the branch
$ git checkout alpha

# Switched to branch 'alpha'

# list of bracnh
$ git branch

- alpha
  master

# crate new brach and switched
$ git checkout -b beta

# Switched to a new branch 'beta'

# list of branch

$ git branch
alpha

- beta
  master

# switch the branch
$ git checkout alpha

# Switched to branch 'alpha'

# create new branch

# creating new file
$ touch style.css

$ git status

$ git add .

$ git status

$ git commit -m "intial"
[alpha e1b923b] intial
1 file changed, 3 insertions(+)
create mode 100644 style.css

git push --set-upstream origin alpha
username
password

and then check to github





# How to pull request and conflict resolve in git hub

$ git pull origin master

# if any conflict so resolve it then

$ git add .

$ git status

$ git push origin master


// delete branch locally
git branch -d localBranchName

// delete branch remotely
git push origin --delete remoteBranchName




# How to merge in Git
- First thing commit the you local master branch then perform command

- for local merge

- $ git merge local branch
- $ git merge product-curd-operation
- Updating c9a484b..e7c4284
- Fast-forward

  
- for checking local merge

- $ git merge local branch
- $ git merge product-curd-operation
- Already up to date.



- for local branch delete


- $ git branch -d localbranch
- $ git branch -d product-curd-operation
- Deleted branch product-curd-operation (was e7c4284).



- for remote branch delete
- $ git push origin --delete product-curd-operation
- To https://github.com/avinash-dewangan/react-redux-shopping-cart-app.git
- [deleted]         product-curd-operation



