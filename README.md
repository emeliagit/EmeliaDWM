# EmeliaDWM
My DWM config, figure having it up here on Github would probably make it a lot more convenient.

-------- How to install --------

After downloading the most recent release from the releases page (https://github.com/emeliagit/EmeliaDWM/releases), extract it into whatever directory you want. I like to extract it to my home directory, but it doesn't really matter where you do it. From here, there are a couple folders that need placing. 

First off, you'll want to place the ".config" folder in your home directory. This should merge with your already existing .config folder, and it should place my Alacritty configuration in it. 

Then, you'll want to place the ".dwm" folder in your home directory. This folder contains an autostart script, which just starts some programs when you login. 

Third, you'll be left with a folder simply called "dwm", that's the actual DWM folder. It contains DWM as well as some patches and modifications I've made to it. You'll have to compile it in order to install it, so configure stuff before compiling it, and compile it every time you make a change. Before compiling it, make sure to place it in your home directory. To compile it, in your terminal, cd into the "dwm" folder included with the release and run "sudo make clean install". This should compile it, and you should not get any errors. If you do get errors, that means that you don't have the proper dependencies installed, so go install those and then compile it.

Last, you'll want to set up a short cut so you can actually log into it (assuming you're using a login manager). This is quite straightforward and very simple. All you have to do is go into /usr/share/xessions and make a file called "dwm.shortcut" using whatever text editor you like. Inside "dwm.shortcut", just put as follows, and you're done:

[Desktop Entry]
Encoding=UTF-8
Name=dwm
Comment=Dynamic window manager
Exec=dwm
Icon=dwm
Type=XSession
