# TMX
tmx is just a bash script I wrote to make my tmux usage easier. It just "abstract" some
of tmux's commands into shorter more intuitive ones.

### Required dependencies
To install tmx you will need to have git installed. And to use it you will need tmux (duh ) with the tmux-resurrect plugin installed and xdotool.

## Installation
Download the installation script and pipe it to bash or whatever your shell is
```sh
sudo curl -sSl https://sfs.thewisepigeon.tech/tmx | sh
```

You can read what that script does by looking in the `install.sh` file in this repo.

## Usage
As I said tmx just maps some nicer commands to some of tmux's ones. 

`tmx version` : Prints tmx current version

`tmx new <session_name>` : Creates a new tmux session using the provided name

`tmx ls` : Lists all current tmux sessions

`tmx save` : Mapped to C-b C-s which is used by tmux-resurrect to save your current session

`tmx restore` : Mapped to C-b C-r used by tmux-resurrect to restore your previously saved session

`tmx kill <session_name>` : Kills a session

`tmx quit` Mapped to C-b d used to exit a tmux session
