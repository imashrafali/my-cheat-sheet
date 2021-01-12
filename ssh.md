# Generating a new SSH key
## Open Git Bash.

Paste the text below, substituting in your GitHub email address.
'''
$ssh-keygen -t rsa -b 4096 -C "your_email@example.com"
'''
This creates a new ssh key, using the provided email as a label.

Generating public/private rsa key pair.
When you're prompted to "Enter a file in which to save the key," press Enter. This accepts the default file location.

Enter a file in which to save the key (/c/Users/you/.ssh/id_rsa):[Press enter]
At the prompt, type a secure passphrase. For more information, see "Working with SSH key passphrases".
Enter passphrase (empty for no passphrase): [Type a passphrase]
Enter same passphrase again: [Type passphrase again]


#Adding your SSH key to the ssh-agent

Ensure the ssh-agent is running:

If you are using the Git Shell that's installed with GitHub Desktop, the ssh-agent should be running.  

If you are using another terminal prompt, such as Git for Windows, you can use the "Auto-launching the ssh-agent" instructions in "Working with SSH key passphrases", or start it manually:  
start the ssh-agent in the background
'''
eval $(ssh-agent -s)
Agent pid 59566
'''
Add your SSH private key to the ssh-agent. If you created your key with a different name, or if you are adding an existing key that has a different name, replace id_rsa in the command with the name of your private key file.

ssh-add ~/.ssh/id_rsa

#Adding SSH to git hub account

Copy the SSH key to your clipboard.

If your SSH key file has a different name than the example code, modify the filename to match your current setup. When copying your key, don't add any newlines or whitespace.

clip < ~/.ssh/id_rsa.pub
 Copies the contents of the id_rsa.pub file to your clipboard
