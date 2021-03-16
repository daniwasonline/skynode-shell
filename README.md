# Skynode Shell

A shell program used for use within my Skynode cluster of servers. It is a collection of programs and Bash scripts, written in Bash and JavaScript. I decided to make this public as I thought that this would be useful for others.

## How do I use Skynode Shell?
Skynode Shell can be used with the binaries or it can be used plain with Node. Skynode Shell is modularised, meaning that it can be used mix-and-match and each module is its' own app, meaning that it can even be used standalone (perhaps with other operating systems, too).

### Installing a Skynode Shell module
To install Skynode Shell's modules, make sure to grab the module's latest release file from [here](https://github.com/Dannnington/skynode-shell/releases/latest/) and install it to `/usr/bin` or `/bin` (somewhere on your PATH). If you know how to use wget or curl, then copy the link to the download and use it in your curl/wget command. For example, to download Skynode Shell v1.0.0's MOTD module with CURL:

```bash
cd /usr/bin
curl -LO https://github.com/Dannnington/skynode-shell/releases/download/1.0.0/skynode-motd
```

Make sure to use root permissions when installing Skynode Shell, as non-root permissions will not work. **You should also make sure to give it execution permissions with `chmod +x`, as it won't work otherwise.**

#### PAM configuration with MOTD
Skynode Shell's MOTD module is currently incompatible with PAM. You can instead create an sshrc file in `/etc/ssh`. Here's an example of an sshrc file being used for the MOTD:
```bash
/bin/skynode-motd
```

Of course, replace `/bin/skynode-motd` with the path to *your* installation of Skynode Shell MOTD.

## Where can I find Skynode Shell binaries?
Skynode Shell binaries can be found [here](https://ci.bean.codes/danny/skynode-shell/-/releases).

### I don't trust these binaries. Can I build the project myself?
Although the binaries don't have any spyware or malware, I can see why you'd want to build yourself. There's a handy little Node app in the `build` directory that'll automatically build the binaries for you. Just run `node [name of build script]` and you'll be on your way! :)