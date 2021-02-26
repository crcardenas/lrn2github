## BASIC COMMANDS ##

$ git init #initialize local git repository
$ git add <file> # add files to index
$ git status # check status of working tree
$ git commit # commit changes in index
$ git push # push to remote repository
$ git pull # pull latest from remote repository
$ git clone # clone repository into a new dir

## git is already installed on ubuntu ##

## to view hidden git files, your directory:
$ ls -a
# add user info to git repository
$ git config --global user.name 'name'
$ git config --global user.email 'user@domain.com'
# next try adding a file to your repository info
# in this case we have a generic HTML file 'index.html'
$ git add index.html
# this will add files to the "cached" that have
# yet to be committed. It will also indicate files
# that are not being tracked.

## if you want to remove a file from staging area you
## can use:
$ git rm --cached <file>
# check that it has been removed with:
$ git status
# you should see this in your untracked file too.
# can also use standard linux lang e.g.:
$ git add *.html
$ git add .

## try making a change to your html file by adding
# some characters or a line break.
# before we had output that stated:
... new file:   index.html ...
# after saving the changes in a text editor we get
... modified:   index.html ...
