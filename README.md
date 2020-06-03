# tmux via snap

You can use this if you want to install tmux via snap.

## Create a snap

To create a snap of tmux git clone this repo and run:
   
   cd snap-tmux
   snapcraft 

To install the local .snap package that you build run `snap install tmux-non-dead_3.1b_multi.snap --devmode`.
In order for it to work you might have to change grade and confinement in snapcraft.yaml. 
