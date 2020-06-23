# tmux via snap

[![tmux-non-dead](https://snapcraft.io//tmux-non-dead/badge.svg)](https://snapcraft.io/tmux-non-dead)

You can use this if you want to install tmux via snap.

## Install this snap

As of now tmux does not seem to work when installed via the snapstore.
Use the instructions below to make a local copy to run.

To create a snap of tmux git clone this repo and run:
   
```shell
   cd snap-tmux
   snapcraft
   sudo snap install tmux-non-dead_[version].snap --devmode
   tmux-non-dead.tmux
```

## Resources

[Releases on GitHub](https://github.com/tmux/tmux/releases)  
[Official development on OpenBSD CVS](https://cvsweb.openbsd.org/cgi-bin/cvsweb/src/usr.bin/tmux/) this is the primary source repository.
Unfortunately snapcraft does not support CVS.  
[tmux mailing list](tmux-users@googlegroups.com)  
[tmux on GitHub](https://github.com/tmux/tmux/wiki)
Things [pledge does](https://github.com/tmux/tmux/blob/master/client.c#L300), might be helpful when locking down slots.
