### Guide

1. Log in to your system as the root user   
    `ssh root@ip`

2. Create a new user account   
    `adduser <username>`

3. Add the new user to the sudo group   
    `usermod -aG sudo <username>`

#### Test the new user sudo access

1. Switch to the newly created user   
    `su - <username>`

2. Use the sudo command to run the whoami command   
    `sudo whoami`

    Is the user have sudo access then the output of the whoami command will be `root`.
