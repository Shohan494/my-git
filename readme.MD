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
	git checkout master
	git merge branch-name

####  
