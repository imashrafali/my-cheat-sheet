#To handle permission denied error--
'''
open windows credential manager
click the github 
and remove the user you want to remove 
'''

#Error-2
'''
 ! [rejected]        master -> master (non-fast-forward)
error: failed to push some refs to 'git@github.com:imashrafali/my-cheat-sheet.git'
hint: Updates were rejected because the tip of your current branch is behind
hint: its remote counterpart. Integrate the remote changes (e.g.
hint: 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.
'''
##solution :
'''
$git checkout master
$git pull --rebase origin master
$git push
'''
optional
'''
$git push --set-upstream origin master
'''