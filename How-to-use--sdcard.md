## Note

The sdcard here means Internal Storage, which is /sdcard, also known as /storage/emulated/0/sdcard, do not be confused with External Sdcard.

To edit sdcard component with AnLinux, you need to edit the start-*.sh script, which is used to start the distro as stated [here:](https://github.com/EXALAB/AnLinux-App/wiki/How-to-start-and-stop-the-distro). 

## Follow the instruction below:

Run this command in Termux to install [nano](https://www.nano-editor.org) editor:

`pkg update && pkg install nano`

Then you must edit the start-*.sh script and uncomment this line:

[#command+=" -b /sdcard"](https://github.com/EXALAB/AnLinux-Resources/blob/master/Scripts/Sample/sample1.sh#L1)