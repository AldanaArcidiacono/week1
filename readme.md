# Learning Git

git init is only use when you create a repo from your local

git checkout HEAD~main : Moves the HEAD where you choose

git reset HEAD~2 : Moves the BRANCH to the commit you choose ##### (Move from the head, x commits behind or you can put the name of the commit EJ: git reset 9565cfbdbd917504a631fcbb5e2c906cfe774ca3 )

We can also find the "futures" commits showing the reflogs (to know the name of the commit) and then, in the terminal with: git reset (name of the commit)

Anything made with JS uses a gitignore of NODE

The first commit is always call "Initial commit"
To clone a repository we press CODE and copy the link under the label HTTPS and paste it on the main folder: git clone (link copied).
After, we go to the new folder that we create with: cd (name of folder).

git add .
git commit -m "(message)"
git push

## Commits

It has 4 parts.
Message
Parent
Name

## Branches

A branch is a LABEL.
I can move it and deleted.
We have infinites branches but only ONE HEAD.
git reset (name of the commit) to put it in the branch we need

## Label HEAD

We can only move it, With the command git checkout
