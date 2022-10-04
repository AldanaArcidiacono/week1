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
Date
The commits are immutable.

## Branches

A branch is a LABEL.
I can move it and deleted.
We have infinites branches but only ONE HEAD.
git reset (name of the commit) to put it in the branch we need
A branch points only to a commit

## Delete a branch

We are just deleting a LABEL
We go to main and use the command git branch -d (name of the branch)

## Label HEAD

We can only move it, With the command git checkout

## Merge

We have to go to our MAIN and then do the command git merge
Git makes a new commit to unite the MAIN (that may change) and your new branch

## Rebase

Also does a MERGE.
At the end, it looks like we made a fast-forward. Because it deletes the commits in the middle and re-write them (we have news commits, since this ones can not change)
It has a cleaner structure, but you can not see when you made a change in other branch

## Resolving conflicts

Conflicts happens when two persons makes changes in the same branch. We have to talk with the other person and decide witch one we should apply.

## Pull Request

To merge a branch with the main.
WE DON'T WORK ON MAIN. (just the initial files)
I ask for a pull and after someone sees it and approves it, is fusion with the main
We take the branches to the remote repo
With this we incorporate from the branch on GitHub to the main of GitHub
git push origin (name of the branch)

## Work flows

Rules to follow that the company decides to use
git flow =
We will use 🔽
gitHub flow = When you made a pull request of a branch, review the pull request. When this is approves, you can merge it and delete the branch. Master always protected. Master always actualized

# Learning HTML

We always have a header and a body on a HTML file
DOCTYPE: tells the program witch HTML you are using <br>
<tag attribute="">
