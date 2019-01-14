## How to start and stop the VNC Server (Desktop Environment)

### Requirement: Distro and Desktop Environment installed

To start VNC Server, run this command:

`vncserver-start`

To stop VNC Server, run this command:

`vncserver-stop`

It is important to run `vncserver-stop` command before closing the distro to exit successfully.

Both `vncserver-start` and `vncserver-stop` scripts are located at /usr/local/bin in the distro, which is corresponding to these file:

[vncserver-start](https://github.com/EXALAB/AnLinux-Resources/blob/master/Scripts/DesktopEnvironment/Apt/vncserver-start)
[vncserver-stop](https://github.com/EXALAB/AnLinux-Resources/blob/master/Scripts/DesktopEnvironment/Apt/vncserver-stop)

You could always modify these file so it could meet your needs.
