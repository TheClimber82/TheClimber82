## How to setup OpenSSH Server

Requirement: SSH Server installed

After running the SSH command provided in the app, sometimes you may not able to use root user to login to SSH Server, as some SSH Client require user to enter a password. This could be solved by creating a new user, login using that user and switch to root then by running `su` command.

To create a new user, run this in the Linux distro:

`adduser`

Then enter username, password, and anything you prefer when prompt.