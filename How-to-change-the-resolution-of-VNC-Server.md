After running the Desktop Environment command, this file is installed to /usr/local/bin in the distro:

[https://github.com/EXALAB/AnLinux-Resources/blob/master/Scripts/DesktopEnvironment/Apt/vncserver-start](https://github.com/EXALAB/AnLinux-Resources/blob/master/Scripts/DesktopEnvironment/Apt/vncserver-start)

When looking at the file, you could see this line:

`vncserver -geometry 1024x768 -depth 24 -name remote-desktop :1`

You could change `1024x768` to your preferred resolution, or change anything that you wanted to.