# snap
Scripts to create snaps.

## tmux

To create a snap of tmux make sure you have the following packages installed:
A working C compiler, make, autoconf, automake, pkg-config as well as libevent and ncurses libraries and headers.
The best way to test if you have a working setup is to follow the guide from tmux and make sure it runs correctly:

    git clone https://github.com/tmux/tmux.git
	cd tmux
	sh autogen.sh
	./configure && make

If it works correctly, you can make snap by running:
   
   cd tmux
   snapcraft 

And thats it.
