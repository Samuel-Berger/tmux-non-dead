# tmux via snap

[![tmux-non-dead](https://snapcraft.io//tmux-non-dead/badge.svg)](https://snapcraft.io/tmux-non-dead)

You can use this if you want to install tmux via snap.

## Install this snap

As of now tmux does not seem to work when installed via the snapstore.
Use the instructions below to make a local copy to run.

To create a snap and install the locally built snap: git clone this repo and run:

```shell
   cd snap-tmux
   snapcraft
   sudo snap install tmux-non-dead_[version].snap --devmode
   tmux-non-dead.tmux
```

## This branch builds against Ubuntu 20.04 (core20)

If the above does not work you probably need to install the edge versions of core and multipass.

```shell
sudo snap switch --edge multipass
sudo snap refresh multipass
sudo snap switch --beta core20
sudo snap refresh core20
```

Try to run `snapcraft` and see if it works.

Currently the build compiles but won't create a snap due to `Failed to generate snap metadata: The specified command 'tmux' defined in the app 'tmux' is not executable.`

## Resources

* [Releases on GitHub](https://github.com/tmux/tmux/releases)  
* [Official development on OpenBSD CVS](https://cvsweb.openbsd.org/cgi-bin/cvsweb/src/usr.bin/tmux/) this is the primary source repository. Unfortunately snapcraft does not support CVS.  
* [tmux mailing list](tmux-users@googlegroups.com)  
* [tmux on GitHub](https://github.com/tmux/tmux/wiki)
* Waiting for [external development](https://forum.snapcraft.io/t/support-for-man-pages/2299) before proceeding on manpages.
* Waiting for [external development](https://github.com/canonical/multipass/issues/1376) before proceeding to build on Raspbery Pi.
https://dashboard.snapcraft.io/snaps/tmux-non-dead/upload/