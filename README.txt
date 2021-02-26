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

## commit changes!
# this function:
$git commit
# opens up a text editor so you can add comments
# or notifications to other folks about the changes.
#I left a line without a hashtag in there which should
#give us a comment.
# the output looks like this:
[master (root-commit) 881282e] nepenthes_lrns2git
 2 files changed, 11 insertions(+)
 create mode 100644 index.html
 create mode 100644 prog.py
# '$ git status' should now indicate that we have nothing
# in our cache to commit

## command line add comment:
$ git commit -m "Changed by nepenthes, 2.26.2021:15:05"
# and the output should look like:
[master 20a0217] Changed by nepenthes, 2.26.2021:15:04
 3 files changed, 45 insertions(+), 1 deletion(-)
 create mode 100644 README.txt

### break point for now... check logs @
$ cat .git/logs/HEAD


## ignore files
# inorder to ignore a file in your git directory
# tell git by creating an invisible file, e.g.
# '.<filename>'
# !!!! that didn't work... uhhh ?!?
ok... comeback to this
