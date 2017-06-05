# Git Commands

#### Basic
	git init
	git commit -m "first commit"
	git remote add origin https://github.com/Shohan494/lstore.git
	git push -u origin master

#### To show latest commit
	git show HEAD

#### To get back to the last commit
	git checkout HEAD filename

#### To unstage a staged file(added via git add). Also brings it back to the last committed phase
	git reset HEAD filename

#### To back back to a commit phase
	git reset #some#log#code

#### Create new branch
	git branch banch-name

#### Switching to a new branch
	git checkout branch-name

#### To include the created branch's changes into the other(master) branch. Basically to keep a balance in between branches, merge is used in git
	git checkout master
	git merge branch-name

#### To get rid of conflict in the same file in different branches, merge conflict appears. To solve this issue, this is called conflict resolve in git. While merging we will see some issues on the file that creates the conflicts between two branches. We can simply get rid of them and after making sure which version we want to keep, then we can add the file and commit

#### After creating a branch, if the branch reaches its target, we can delete the branch if we want
	git branch -d branch_name

#### To clone a repo from a remote location and to give it a new name
	git clone remote_location clone_name

#### To list the remotes
	git remote -v

#### To fetch any new changes that may have made to the remote
	git fetch

#### If some changes are made in the origin/master, we can merge with the local/master repo to remote(origin/master) repo
	git merge origin/master

#### After merging with the origin/master repo, if we create a new branch for our own project, we can create, work on it, then we can push the branch to the origin/master repo. So the steps will be basically:
- Creating a new branch
- Then working on the project, adding files, commiting etc
- Then we can push the branch to origin/master via:
	
		git push origin your_branch_name

#### To apply cherry-pick command, we have to make sure in which branch we will apply, then simply pick a hash
	git checkout branch-name
	git cherry-pick <commit-hash>

## Git Stash

#### For a temporary save we can use stash command. Like after some changes that we have made and we are not sure to make it permanent, then making a stash command and switching to other work
	git stash
#### To provide some more info and then save the stash
	git stash save "message"

#### To re-apply and drop the stash, this command will remove the latest one
	git stash pop
#### To remove a specific stash
    git stash pop stash@{2}
#### To apply and keep them on stash
	git stash apply

#### We can stash multiple times. So to have a list of stashes
	git stash list

#### To stash ignored files also
	git stash -u

#### We can view the stash diffs
	git stash show

#### Partial stashing(individual or all files)
	git stash -p

#### Drop a particular stash
	git stash drop stash@{1}

#### Clear all stash
	git stash clear

#### To view our each commit(basically git log) to a single line, we can use
	git log --oneline

#### To view added or removed lines(basically diffs) we can use
	git log --stat
	git log -p

#### To view commits based on authors
	git shortlog

#### log history with or without merges
git log --merges
git log --no-merges