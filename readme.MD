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

#### To merge with the local repo to remote repo
	git merge origin/master