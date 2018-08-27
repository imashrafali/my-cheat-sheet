# Use full git commands
'''
$git status
$git add -A, . for staging
$git commit -m "name"  committing
'''
# To connect to git origin i.e git hub
'''
$git add remote origin
$git pull origin master
$git push origin master
$git push -u origin master
'''
# To check log we use
$ git log

# TO check overall changes git/git hub
'''
$ git pull origin master
$ git log
'''  

# To scan changes in the file we use diff commnad

$ git diff 'filename'

# To scan changes if the file is in staging

$ git diff --staged 'filename'

# To unstaged the changes in the file to return it to old state

$ git reset 'filename'

# TO remove the change in the file

$git checkout 'filename'
  
for multiple files
$git checkout .

cloning A git Repository it creates a folder

$git clone "SSH url"

instead of folder to create a repo
$git clone "ssh url" .

<<<<<<< HEAD
#to ignore specific files in git
$touch .gitignore it creates a empty file
$notepad .gitignore
=======
>>>branches in git

$git branch
$git branch filename
$git checkout filename
$git push origin branchname

>>>To return to master
$git checkout master

Merging 2 branches
$git merge 'name of the branch you want to merge to master'
>>>>>>> test

>>>>>>>To delete the branch locally

$git branch -d 'branchname' -->to delete locally

>>>>>>>To delete branch of github from the gitbash

$git push origin --delete 'branchname'
