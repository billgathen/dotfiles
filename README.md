My current dotfile setup, taken in large part from Geoffrey Groesenbach's [Advanced Command-Line](https://peepcode.com/products/advanced-command-line) PeepCode screencast.

To use this on your Unix system (I'm on OSX):

1. First, fork your own version of this project using the **Fork** button at the top of the page. Then you can change it however you like and store the changes on Github.
1. Click the **Copy to clipboard** icon at the top of the page in your new repository.
1. In your terminal, `cd ~/bin`. Create the dir with `mkdir ~/bin` if you don't already have it.
1. Type `git clone`, paste in the URL you got from above, then press enter. This will insert everything into `~/bin/dotfiles`.
1. `cd ~`
1. `ls -a ~/bin/dotfiles/examples` will reveal the 4 files I keep so I can use either shell (bash or zsh) with largely the same feature set.
1. Back up your existing ones first. I suggest `mv .bashrc .old_bashrc`, etc.
1. Copy the 2 that match your shell (or all 4 if you like) into your home directory with `cp ~/bin/dotfiles/examples/.bashrc .`, etc.

The next time you open a terminal window, you should get all the features.

If you're on one shell (probably bash) and want to try the other, use `chsh -s /bin/bash` or `chsh -s /bin/zsh` (whichever you want to try out) at the command line. You'll have to open a new terminal window to see the change, but now you're good to go!

**NOTE** `~/bin/dotfiles/shell_config/env` has a `source ~/.auth` line, which loads my auth credentials for the various things I do. Make sure you do the same (instead of putting them directly in that file) in order to prevent your passwords from showing up on Github! ;-)