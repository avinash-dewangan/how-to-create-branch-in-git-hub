#How to Create branch in git hub common line

\$ git status

//create new branch
\$ git branch alpha

//list of branch
\$ git branch --list
alpha

- master

//swich the branch
\$ git checkout alpha
Switched to branch 'alpha'

// list of bracnh
\$ git branch

- alpha
  master

//crate new brach and switched
\$ git checkout -b beta
Switched to a new branch 'beta'

// list of branch

\$ git branch
alpha

- beta
  master

//switch the branch
\$ git checkout alpha
Switched to branch 'alpha'

//create new branch
#creating new file
\$ touch style.css

\$ git status

\$ git add .

\$ git status

\$ git commit -m "intial"
[alpha e1b923b] intial
1 file changed, 3 insertions(+)
create mode 100644 style.css

git push --set-upstream origin alpha
username
password

and then check to github
