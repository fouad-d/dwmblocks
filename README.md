# dwmblocks

Modular status bar for dwm written in c.

My dwmblocks config
The statusbar is made from text output from scripts found in my .local/bin.  Blocks are added and removed by editing the blocks.h header file.

To get my dwmblocks to work for you...

You will, of course, need my dwmblocks build and my scripts in .local/bin.  Make sure that .local/bin is in your $PATH otherwise you can't call those scripts by name which is what I'm doing in blocks.h.  Instead, you'd have to write out the full path to each script in the blocks.h.

To add .local/bin to $PATH, just add this line to your .bashrc:
PATH="$HOME/.local/bin${PATH:+:${PATH}}"

Clickable modules
Like i3blocks, this build allows you to build in additional actions into your scripts in response to click events. See the above linked scripts for examples of this using the $BLOCK_BUTTON variable.

For this feature to work, you need the appropriate patch in dwm as well. See here. Credit for those patches goes to Daniel Bylinka (daniel.bylinka@gmail.com).

So if you want my build out of the box, download those and put them in your $PATH .

