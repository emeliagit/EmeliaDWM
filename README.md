# EmeliaDWM
My DWM config, figure having it up here on Github would probably make it a lot more convenient.

-------- How to install --------

After downloading the most recent release from the releases page (https://github.com/emeliagit/EmeliaDWM/releases), extract it into whatever directory you want. I like to extract it to my home directory, but it doesn't really matter where you do it. From here, there are a couple folders that need placing. 

First off, you'll want to place the ".config" folder in your home directory. This should merge with your already existing .config folder, and it should place my Alacritty configuration in it. 

Then, you'll want to place the ".dwm" folder in your home directory. This folder contains an autostart script, which just starts some programs when you login. There's also a line in the "autostart.sh" script that adjusts for my own display, you'll want to delete that line (or comment it out).

Third, you'll be left with a folder simply called "dwm", that's the actual DWM folder. It contains DWM as well as some patches and modifications I've made to it. You'll have to compile it in order to install it, so configure stuff before compiling it, and compile it every time you make a change. Before compiling it, make sure to place it in your home directory. To compile it, in your terminal, cd into the "dwm" folder included with the release and run "sudo make clean install". This should compile it, and you should not get any errors. If you do get errors, that means that you don't have the proper dependencies installed, so go install those and then compile it.

Last, you'll want to set up a short cut so you can actually log into it (assuming you're using a login manager). This is quite straightforward and very simple. All you have to do is go into /usr/share/xessions and make a file called "dwm.shortcut" using whatever text editor you like. Inside "dwm.shortcut", just put as follows, and you're done:

[Desktop Entry]
Encoding=UTF-8
Name=dwm
Comment=Dynamic window manager
Exec=dwm
Icon=dwm
Type=XSession

-------- Additional dependencies --------

Beyond the normal dependencies for DWM, there are some more required to get my configuration to really work. They are as follows:
- dmenu
- picom
- nitrogen (optional, for setting wallpaper)
- caffeine (optional)
- xfce4-power-manager
- networkmanager

Some screenshots for the curious: 
file:///home/emelia/Pictures/Screen%20Shots/Screenshot_2022-07-21_18-30-26.png![image](https://user-images.githubusercontent.com/66752943/180325986-0929fed5-b623-4d2a-a9fe-7361431f267a.png)

file:///home/emelia/Pictures/Screen%20Shots/Screenshot_2022-07-21_18-29-17.png![image](https://user-images.githubusercontent.com/66752943/180326030-2bdea24c-61c0-4153-a38e-ce1ecbb88174.png)
