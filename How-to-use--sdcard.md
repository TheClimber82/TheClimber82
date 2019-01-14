## Note

### Requirement: Distro installed

The sdcard here means Internal Storage, which is /sdcard, also known as /storage/emulated/0/sdcard, do not be confused with External Sdcard, please make sure you have granted Termux Storage permission before doing this, if not sure, view Termux's permission in App Info.

To edit sdcard component with AnLinux, you need to edit the start-*.sh script, which is used to start the distro as stated [here:](https://github.com/EXALAB/AnLinux-App/wiki/How-to-start-and-stop-the-distro). 

## Follow the instruction below:

1. Download [Hacker's Keyboard](https://play.google.com/store/apps/details?id=org.pocketworkstation.pckeyboard&hl=en) and switch to [Hacker's Keyboard](https://play.google.com/store/apps/details?id=org.pocketworkstation.pckeyboard&hl=en).

2. Run this command in Termux to install [nano](https://www.nano-editor.org) editor:

    `pkg update && pkg install nano`

3. Then you must edit the start-*.sh script and uncomment this line:

    `#command+=" -b /sdcard"`

   so it become:

    `command+=" -b /sdcard"`

4. Press CTRL + X and then press y, then press ENTER to save the file.

5. You can now launch distro with the new start-*.sh script, it will automatically mount /sdcard in the distro.
