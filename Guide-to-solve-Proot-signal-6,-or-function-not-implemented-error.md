Main reason that cause this is SECCOMP, so put this command in Termux .bashrc and restart it would solve it:

`echo "export PROOT_NO_SECCOMP=1" >> .bashrc`