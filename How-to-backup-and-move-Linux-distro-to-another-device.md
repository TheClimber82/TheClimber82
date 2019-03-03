First of all, if you don't know yet, the distro is located at /data/data/com.termux/files/home.

If it is Ubuntu, the folder is /data/data/com.termux/files/home/ubuntu-fs,  if it is Arch Linux, the folder is /data/data/com.termux/files/home/arch-fs , same for the rest, you can find the folder by running ls command.

Let's take Ubuntu for example:

If you look at this file: [ubuntu.sh](https://github.com/EXALAB/AnLinux-Resources/blob/master/Scripts/Installer/Ubuntu/ubuntu.sh), you would found out the installer file create three things:

1. ubuntu-fs

2. ubuntu-binds

3. start-buntu.sh

Now let's start backup!

1. Open Termux, and run `pkg install tar` if you haven't done yet.

2. Run this command to backup Ubuntu: `tar -cvf backup-ubuntu.tar.gz ubuntu-fs ubuntu-binds start-ubuntu.sh`

3. Then you may need to copy backup-ubuntu.tar.gz to sdcard, to do this, run this command: `cp backup-ubuntu.tar.gz /sdcard`

4. Transfer the file to sdcard of new device.

5. Open Termux and install tar following step 1.

6. Run this command to copy backup file into Termux directory: `cp /sdcard/backup-ubuntu.tar.gz /data/data/com.termux/files/home`

7. Extract it and remove the backup file: `tar -xzvf backup-ubuntu.tar.gz && rm backup-ubuntu.tar.gz`

8. Run your distro by using `./start-ubuntu.sh`