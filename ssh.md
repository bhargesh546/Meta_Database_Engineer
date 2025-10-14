# Generating SSH
* Open the terminal
* Enter the following:
    > `ssh-keygen -t ed25519 -C "your@email.com"`
* It will prompt to enter a password. Hit enter to skip setting a password and do the same for entering the same passphrase again.
* Once you have confirmed it will generate the above to confirm the keys have been created.  
Both keys will be stored in the **.ssh** folder.
* In order to add our key to Github, we need to get a copy of the public key which is always identified as .pub in your local directory.  
Find the name of the key file using the below command.  
`ls ~/.ssh/`  
Then, use the below command to copy the file, replacing the \<YOUR KEY\> with the name of the key file on your device. This step differs between Windows and Mac.  
For Windows:   
`cat ~/.ssh/<YOUR KEY>.pub | clip`   
For Mac:  
`pbcopy < ~/.ssh/<YOUR KEY>.pub`

* Finally add your Keys to Github

You are now ready to access Github via SSH.