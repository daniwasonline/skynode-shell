# Sysinfo
This is a drop-in replacement for Ubuntu's Landscape Sysinfo tool, intended for use in CentOS, Fedora, and RHEL systems (although it'll work on just about any other Linux system). It is intended to be cross-compatible with other platforms, so Darwin- and Windows-based systems have compatibility with this tool.

## How do I install Sysinfo?
Skynode Sysinfo can be installed by simply placing it into a PATH-covered directory (/bin, /usr/bin, etc.), then adding an entry for it in your dynamic MOTD directory (Ubuntu's update-motd.d, Skynode MOTD, or another dynamic MOTD solution). If you are using Ubuntu's update-motd, then you will create a file in `/etc/update-motd.d`. If you are using Skynode MOTD, then you will create a file in `/etc/skynode/motd.d`. The content of the file will contain the following:
```sh
#!/bin/sh
/bin/skynode-sysinfo
```

Of course, replace `/bin/skynode-sysinfo` with YOUR path to Sysinfo.

You will notice the change on next login.
Enjoy!