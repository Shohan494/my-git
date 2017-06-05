# Git Commands

#### Basic

	git init
	git commit -m "first commit"
	git remote add origin https://github.com/Shohan494/lstore.git
	git push -u origin master

#### to show latest commit
	git show HEAD

#### to get back to the last commit
	git checkout HEAD filename

#### to unstage a staged file(added via git add)
#### also brings it back to the last committed phase
	git reset HEAD filename

#### to back back to a commit phase
	git reset #some#log#code

#### create new branch
	git branch banch-name

#### switching to a new branch
	git checkout branch-name

#### to include the created branch's changes into the other(master) branch
#### basically to keep a balance in between branches, merge is used in git
	git checkout master
	git merge branch-name

#### to get rid of conflict in the same file in different branches, merge conflict appears
#### to solve this issue, this is called conflict resolve in git
#### while merging we will see some issues on the file that creates the conflicts between two branches
#### we can simply get rid of them and after making sure which version we want to keep, then we can add the file and commit

