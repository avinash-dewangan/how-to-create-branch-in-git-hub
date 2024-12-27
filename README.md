
    
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

# If User setting user name and password
- $git config --global user.name "fname lname"
- $git config --global user.email "example@gmail.com"
- $git config --global user.password "secret"

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


# How to push master branch when currently dev branch
- First commit dev branch
- $ git push origin dev
- then commit master branch below command
- $ git push origin dev:master


# CheckOut old  Commited Checkout
 git checkout a1f5e04
 
# Stash
 for revert changes

## Steps to Override master with dev:

Switch to the dev branch:
```
git checkout dev
```
Force push dev to master:
```
git push origin dev:master --force
```
This command pushes the dev branch to the master branch on the remote, overwriting the existing history.

Alternatively: Merge dev into master (Safer Approach)
If you want to preserve the master branch history, you can merge the dev branch instead of overriding:

Switch to master:

```
git checkout master
```
Merge dev into master:
```
git merge dev
```
Push the changes to the remote:
```
git push origin master
```

# Reverting Local Changes in Git

## **1. Revert Unstaged Changes (Unmodified Files)**
If you have made changes to files but have not staged them (using `git add`), you can discard them:

```bash
git restore <file-name>
```

To discard changes to all files:
```bash
git restore .
```

---

## **2. Revert Staged Changes**
If you have staged changes (added them to the index using `git add`), you can unstage them:

```bash
git reset HEAD <file-name>
```

To unstage all changes:
```bash
git reset HEAD .
```

---

## **3. Revert to the Last Committed State**
If you want to discard **all changes** (both staged and unstaged) and revert the working directory to the last committed state:

```bash
git reset --hard HEAD
```

---

## **4. Revert Changes to a Specific Commit**
If you want to undo changes back to a specific commit but keep your working directory clean:

```bash
git reset --hard <commit-hash>
```

---

## **5. Undo a Specific File to Last Commit**
If you want to revert a specific file to the last committed state:

```bash
git checkout -- <file-name>
```

---

## **6. Revert a Commit (Without Losing Changes)**
If you've already committed the changes but want to revert them without losing the history, use:

```bash
git revert <commit-hash>
```

This creates a new commit that reverses the changes of the specified commit.

---

## **Important Notes:**
- Be careful with `git reset --hard` and `git checkout --` as they will permanently discard your changes.  
- Always ensure that any important changes are saved or backed up before reverting.


