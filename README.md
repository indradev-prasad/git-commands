# Some important commands of git
```sh
#Config
#Identity
$ git config --global user.name "John Doe"
$ git config --global user.email johndoe@example.com
#Set Editir
$ git config --global core.editor emacs
#List of config
$ git config --list
#Individual
$ git config user.name
#Initialize
#Non existing repository
$ git init
$ git add *.c #(all c file)
$ git add LICENSE #licence file
$ git commit -m 'initial project version'
#Existing repository
$ git clone https://github.com/libgit2/libgit2
#create own folder
$ git clone https://github.com/libgit2/libgit2 mylibgit
#Pass user name as well
$ git clone https://{{user}}@github.com/libgit2/libgit2 
#clone to root directory
$ git clone https://github.com/libgit2/libgit2 -
#Clone with Branch
$ git clone -b opencv-2.4 --single-branch https://github.com/libgit2/libgit2
#Basic commond
$ git status
$ git status -s (short)
$ git add <filename>
$ git add . #all
$ git add -all 
$ git rm <filename> 
$ git rm --cached <filename> #remove from only track not from hard drive. most time .gitignore file
$ git rm -f <filename>
$ git mv <from_file> <to to_file> #(Rename the file name)
$ git diff #check what you have made difference from last commit
$ git checkout <filename> #get from commit
$ git reset <filename> #remove stage file. added file

#commit history
$ git log
$ git log -p #patch
$ git log -p -2{number of commits}
$ git log --stat
$ git log --stat
$ git log --pretty=oneline
#Link :https://git-scm.com/book/en/v2/Git-Basics-Viewing-the-Commit-History
#Undoing Things
$ git commit --amend #add additional file to last commit
#Unstaging a Staged File
$ git reset HEAD <filename>
$ git checkout -- <filename>
#Working with Remotes
$ git clone https://github.com/schacon/ticgit
$ git remote
$ git remote --v
#Add git remote
$ git remote add <shortname> <url>
$ git remote add pb https://github.com/paulboone/ticgit (given short name as pb)
$ git fetch pb
$ git fetch <remote>

#Push
$ git push origin master #Branch Name
#Pull
$ git pull origin master #Branch Name

#git branch
$ git log --oneline --decorate
$ git log --oneline --decorate --graph --all
$ git branch <branchname> #Create branch
$ git checkout <branchname>  #switch to branch
$ git merge <branchname> #merge one branch to other
$ git branch --v
$ git branch --merged
$ git branch -d <branchname> #delete branch
```

See More [https://git-scm.com/book/](https://git-scm.com/book/)

