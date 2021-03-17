# PS/1

## WARNING!
Skynode PS/1, unlike MOTD and Sysinfo, should NOT be used in production environments. It may cause harm to its' surrounding environment and may malfunction easily. With that being said, binaries have not been built for Skynode PS/1 as it may be considered dangerous to critical environments like production or stable. **No build scripts have been provided for PS/1 either.** It has only been left in the Shell repository for archival and development purposes.

## Description
This is intended to be a "replacement" (see warning above for why it is not a real replacement) for the standard PS/1 variable, written in Node.js. It has a more recognisable colour syntax (albeit more hefty to use) and it has some of the common-place use-features that regular PS/1 provides! It can also inter-twine with standard PS/1, for more flexibility and usability. 

### WARNING! (2)
Skynode PS/1 does not provide a proper \\w variable. Due to how Bash variables work, unless if a daemon was used to track a current directory and then dynamically update the PS/1 variable, it would be nearly impossible to implement a \\w variable.