# tmux via snap

[![tmux-non-dead](https://snapcraft.io//tmux-non-dead/badge.svg)](https://snapcraft.io/tmux-non-dead)

You can use this if you want to install tmux via snap.

## Create a snap

To create a snap of tmux git clone this repo and run:
   
```shell
   cd snap-tmux
   snapcraft
   snap install tmux-non-dead_3.1b_multi.snap --devmode
```

To install the local .snap package that you build run `snap install tmux-non-dead_3.1b_multi.snap --devmode`.
In order for it to work you might have to change grade and confinement in snapcraft.yaml.

## Resources

[Releases on GitHub](https://github.com/tmux/tmux/releases)  
[Official development on OpenBSD CVS](https://cvsweb.openbsd.org/cgi-bin/cvsweb/src/usr.bin/tmux/) this is the primary source repository.
Unfortunately snapcraft does not support CVS.  
[tmux mailing list](tmux-users@googlegroups.com)  
[tmux on GitHub](https://github.com/tmux/tmux/wiki)
