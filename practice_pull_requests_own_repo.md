Practice pull request on your own repository
================
Ariel Muldoon
7/22/2019

  - [Make a new branch](#make-a-new-branch)
  - [Make commit and push](#make-commit-and-push)
  - [Make pull request on GitHub](#make-pull-request-on-github)
      - [Continue making commits](#continue-making-commits)
  - [Merge](#merge)
  - [Pull to local repo](#pull-to-local-repo)
  - [Delete local branches](#delete-local-branches)

See an example of making a pull request to your own repository
[here](https://r-pkgs.org/git.html#git-pullreq) in the R Packages book.

# Make a new branch

Pull requests are simplest when making a pull request to your own
repository. The first step is to make a new branch. If you have no
collaborators or if all collaborators work via pull requests you
generally won’t need to worry about things on the repo changing while
you’re working (these are called “upstream changes”). This makes the
process a little more streamlined.

If using RStudio you can make a new branch within the RStudio Git pane.
You can also do this on GitHub (if you do this on GitHub remember to
Pull to your local repository). And of course there are shell commands
you can use, which I’m not covering here.

Be sure to switch to new branch locally and start editing your first
file.

# Make commit and push

Commit any changes and push up to the branch. You can commit as many
times as you want into the same pull request.

# Make pull request on GitHub

When you go to your repository on GitHub you will see a “Compare and
pull request” button. Push this button and write a description of what
is in your pull request. If you don’t know the full extent of the pull
request yet, no worries. You can add additional comments to the pull
request as you go.

## Continue making commits

You can merge the pull request into the master branch right away if you
want. You can also continue to make commits and push to the branch. All
changes will be added to the same pull request for that branch.

# Merge

When you’re done for the day or done with a particular set of edits,
merge your pull request to the master branch on GitHub. You’ll be given
the option to delete the branch you were working on, which is
recommended. Your next task can be done in a new branch with a new pull
request.

# Pull to local repo

When you’ve merged all changes, go back to the master branch in RStudio
and pull in the changes.

# Delete local branches

RStudio doesn’t have a point-and-click method for deleting local
branches. See [this
thread](https://community.rstudio.com/t/delete-branch-in-rstudio-pop-up/15465).

To delete the branch locally, open the shell/terminal and type `git
branch -d branchname`

To delete the remote origin branches use `git fetch -p`
