Editing Commits with Git
========================
This is a companion repository for the [post on my
blog](http://journal.ryanmccue.info/202/editing-commits-with-git/).


How do I try this out?
----------------------
This branch that you're reading at the moment is the master branch. We want to
merge the `fixes` branch back into this branch.

The problem is that we accidentally misspelled a word in the second commit that
we want to pull from `fixes`. We could fix this after the fact with a new
commit, but we might as well fix it in that commit.

Here's how to fix it:
* Switch to the fixes branch (in a real repository, we'd pull in the remote
  here, but you should already have it)
* Run an interactive rebase on the previous three commits
* Change the second commit to `edit`
* Edit the file to fix the mistake
* Amend the commit
* Continue the rebase


Checkin' It Twice
-----------------
If you think you've sorted it out, awesome! Fork my repository, push your new
master up and file a pull request. I'll take a look and check your work. :)
