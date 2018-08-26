# My errors in git and solutions 

## To handle permission denied error

1. open windows credential manager  
2. click the github   
3. remove the user you want to remove 


## Error-2

<b> ! [rejected]        master -> master (non-fast-forward)
error: failed to push some refs to 'git@github.com:imashrafali/my-cheat-sheet.git'
hint: Updates were rejected because the tip of your current branch is behind
hint: its remote counterpart. Integrate the remote changes (e.g.
hint: 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.
<b>
  
## solution :

    $ git checkout master
    $ git pull --rebase origin master
    $ git push
    
#### optional

    $ git push --set-upstream origin master

