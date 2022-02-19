# tmux via snap

[![tmux-non-dead](https://snapcraft.io//tmux-non-dead/badge.svg)](https://snapcraft.io/tmux-non-dead)

You can use this if you want to install tmux via snap.

## Install on your Local Machine

If you want to use `tmux` instead of `tmux-non-dead` you have to build and install from your local machine. First change the first line in `snapcraft.yaml` from `tmux-non-dead` to `tmux`.
Then build it locally.

To create a snap and install the locally built snap: git clone this repo and run:

```sh
   cd snap-tmux
   snapcraft
   sudo snap install tmux-non-dead_[version].snap --devmode
   tmux-non-dead.tmux
```

## How to Build and Release

```sh
snapcraft
snapcraft login   # You won't be able to do this step.
snapcraft upload tmux-non-dead_3.2a_multi.snap --release candidate, beta
sudo snap install tmux-non-dead --candidate --classic
```

## Resources

* [Releases on GitHub](https://github.com/tmux/tmux/releases)  
* [Official development on OpenBSD CVS](https://cvsweb.openbsd.org/cgi-bin/cvsweb/src/usr.bin/tmux/) this is the primary source repository. Unfortunately snapcraft does not support CVS.  
* [tmux mailing list](tmux-users@googlegroups.com)  
* [tmux on GitHub](https://github.com/tmux/tmux/wiki)
* Waiting for [external development](https://forum.snapcraft.io/t/support-for-man-pages/2299) before proceeding on manpages.
* Waiting for [external development](https://github.com/canonical/multipass/issues/1376) before proceeding to build on Raspbery Pi.
https://dashboard.snapcraft.io/snaps/tmux-non-dead/upload/