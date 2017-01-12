git init --> initializes and creates a git repository in the folder you have executed the command.

git add `filename(s)` --> adds the multiple files to the staging area, the plca they are put before they are actually commited to the repository.

git status --> provides info about tracked and untracked files from the project.

git status -s or git status --short --> provides the brief information on the tracked and untracked files.

git commit --> to push the files to the repository, an editor will be displayed for you enter the message

git commit -m "Comment to be added" --> to push the files to the repository

git commit -a -m "Comment to be added" --> to push the files to the repository.

git diff --> will display the changes made in  the staged files.

git rm --cached <filename> --> Removes the file from the staging area and places it back to the unstaged area.

To remove a file completely :
rm `filename`
git rm --cached `filename`
git commit --> the repository will stop tracking the file changes for the file `filename`

renaming files or moving files to directory :

git mv README.md README - this command is equivalent to executing the following:

mv README.md README
git rm README.md
git add README

git log --> provides the complete history of changes, with info such as the SHA-1 hash value, Author and the date.
git log -p -n -->  provides the complete history of change, but now it provide the file differences as well. -n options allow you control the number of logs that must be output.

git log pretty:oneline/short/full/fuller

git pretty=format:"%h %an %ad %s" --> prints the hash value, author name, author date and the comments



How to add a remote to your repository ?
$ git remote add origin https://github.com/gitusername/gitleraning 

This will just add a remote git repository to your local git setup. I will push this repository to the github.
Now create a remote repository in github to push the local repository to it. Once done, do the following - 

$ git push origin master

This will ask you for github username and password.





