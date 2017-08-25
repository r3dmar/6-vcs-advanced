# 6-vcs-advanced

##Tsk 1
--------
git clone https://github.com/r3dmar/git-advanced-hw2.git
cd /c/Users/admin/git-advanced-hw2
git init
git checkout -b architecture
touch index.html
mkdir assets
mkdir uploads
git status
git add .
git commit -m "adding index.html and structure folders"
cd /c/Users/admin/git-advanced-hw2/assets
touch all.js
touch css.js
git status
git add . 
git status
git commit -m "adding 2 files (all.js and css.jss) in folder assets"
cd /c/Users/admin/git-advanced-hw2/uploads
touch .gitignore
	than add in to .gitignore file text 
		"# Ignore everything in this directory
		*
		# Except this file
		!.gitignore"

git commit -m "add .gitignore file in to folde uploads for always empty folder"
git push -u origin architecture
git checkout master
git merge architecture
git branch
git branch -d architecture



## Tsk2
-------
git branch rb
touch index.css
git add .
git commit -m "add new index.css file"
git add .
git commit -m "add new text-info in to index.css"
git branch
git checkout rb
git branch
git rebase master
touch shit.txt
git add .
git checkout master
git commit -m "added shit.txt file"
git merge rb
git branch -d rb


## Tsk 3
--------------
mkdir img
(then add texture.img)
git add .
git commit -m "added /img folder and texture img"
(delete old texture.img and add new)
git add . 
git commit -m "change texture.img"
git tag -a v1.0 -m "my version 1.0"
git push

## Tsk 4
-------------
git submodule add https://github.com/r3dmar/ihover.git ihover
git status
gitcommit -m "added new submodul ihover (css features)"
git push

## Tsk 5
-------------------
git checkout -b gh-pages
echo "Hello World" > index.html
git status
git add .
git commit -m "add new index.html with Hello World text
	in to index.html add pic texture.jpj"
git status
git add .
git commit -m "modified index.html file, add img in to"
git push -u origin gh-pages

## Task 6
--------------
echo "Hello my little friend" >> test.txt
git status
git add .
git commit -m "added test.txt"
git push
git checkout -b cursorconflict
git status
git add .
git commit -m "updated test.txt in cursorconflict branch"
git push -u origin cursorconflict
git checkout master
git merge task-6
	(Auto-merging test.txt
	CONFLICT (add/add): Merge conflict in test.txt
	Automatic merge failed; fix conflicts and then commit the result.)
git merge --abort
git status
git add .
git commit -m "merging confict files"
git status
git push
-------------------


