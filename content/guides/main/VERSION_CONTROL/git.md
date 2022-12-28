# git
---
[git tutorial - Corey Shafer](https://www.youtube.com/watch?v=HVsySz-h9r4)

arch -> `s`
gentoo -> `dev-vcs/git`

---

check version
```
$ git --version
```

set global config variables
```
$ git config --global user.name "Benjamin Dunstan"
$ git config --global user.email "benjadunstan@gmail.com"
$ git config --list
```

help command
```
$ git help config
or
$ git config --help
```

---

initialize a repository from existing code
```
$ git init
```

to stop tracking a repository, you can remove the `.git` folder inside that repository
```
$ rm -rf .git
```

__starting__
before first commit, do this, to check what files are going to be commited and if there's a file or personal information to ignore
```
$ git status
```

ignore files or directories creating this next file
```
$ touch .gitignore
```
this is a simple text file, add what you want to ignore, you can also use wildcards.
__EXAMPLE__ (in `.gitignore`)
```
.DS_Store
.project
*.pyc
```
we want to commit the `.gitignore` file so the repository can know which files to commit.

![[Pasted image 20221226135009.png]]

__staging area__
add all the files
```
$ git add -A
or for a individual file
$ git add <file>
```

remove files from staging area
```
$ git reset
or for a individual file
$ git reset <file>
```

__commit__
start your first commit with:
```
$ git commit -m "<message"
```

__log__
check the log, which displays the hash of the commit, the date and author
```
$ git log
```

__cloning__
clone a remote repository with this
```
$ git clone <url> <directory>
```
if you don't use a directory, it will create one with the repo name, if you specify a directory, it will extract the files there

view information about a remote repository
```
$ git remote -v
$ git branch -a
```

__pushing changes__
check the modified files 
```
$ git diff
$ git add -A
$ git commit -m "Added an extra functionality"
```

pull then push
- pull: is important as it will pull any changes on the repository
```
$ git pull origin master
then
$ git push origin master
```

__creating a brach__
in case of adding a desired feature, we can create a branch to work on it
```
$ git branch <branch-name>
```
just typing `git branch`, will output your local branches. The asterisk means the branch you're currently working on.

Change to a different branch
```
$ git checkout <branch-name>
```

add to staging area, commit, push branch to remote
```
$ git add -A
$ git commit -m "Added from <branch-name> :)"
$ git push -u origin <branch-name>
$ git branch -a
```

let's move to master branch again
```
$ git checkout master
```

__merge a branch with master__
remember to always pull
```
$ git pull origin master
```
run the next command, to see which branches have been merged
```
$ git branch --merged
```
merge the branch !
```
$ git merge <branch-name>
```
now push the changes :3
```
$ git push origin master
```

__ERROR fix__
branch is currently checked out
- go back to your original folder, which should be running under the main branch
- create a dummy branch with
```
$ git checkout -b dummy
```
- go back to your remote branch and push

__deleting a branch__
check if everything was correctly merged by
```
$ git branch --merged
```
you should see your branch above the master branch.

delete the branch
```
$ git branch -d <branch-name>
```

we also pushed that branch to remote repo, so we need to delete it from there too
check the branches
```
$ git branch -a
```

remove it with:
```
$ git push origin --delete meow1
```

---

a routine workflow
```
$ git branch test
$ git checkout test
modify file
$ git add -A
$ git commit -m "Added X"
$ git push -u origin test
$ git checkout master
$ git pull origin master
$ git merge test
$ git push origin master
```
