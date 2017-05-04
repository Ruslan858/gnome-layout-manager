### Notice: This software is alpha and under development. Please use at your own risk.


# GNOME Layout Manager

### _New feature_: Due to many people asking me, I added a Save/Load function. It's still experimental and a bit slow but should work. It iterates through all gsettings and saves them on a text file in ```~/.config/gnome-layout-manager```  
![Menu](http://i.imgur.com/i5fR098.png)

A bash script that batch installs and tweaks GNOME extensions as well as GTK/Shell themes. There are currently three options available: Unity, Windows and macOS.

To get and run the script:
```
wget https://raw.githubusercontent.com/bill-mavromatis/gnome-layout-manager/master/layoutmanager.sh
chmod +x layoutmanager.sh
./layoutmanager.sh
```
#### Install folders:
Extensions: ```~/.local/share/gnome-shell/extensions```   
Themes: ```~/.themes```  
Icons: ```~/.local/share/icons```  
Schemas: ```~/.local/share/glib-2.0/schemas```  
Wallpaper: ```~/Pictures``` (or as set by xdg-user-dir)  
Backup: ```~/.config/gnome-layout-manager```  

## Unity

Preview: 
![Unity](http://i.imgur.com/He66ZsK.png)
Extensions:
- Dash to dock
- TopIcons Plus
- AppIndicator
- User Themes
- Hide Activities
- Frippery Move Clock

Theme:
- [United (GTK+Shell+Wallpaper)](https://www.gnome-look.org/p/1174889) by [@godlyranchdressing](https://github.com/godlyranchdressing) Licence: GPLv2
- [Humanity icon theme](https://launchpad.net/humanity) by Canonical, Licence: GPLv2

## Windows

Preview: 
![Windows](http://i.imgur.com/W5NIINx.png)

Extensions:
- Dash to panel
- TopIcons Plus
- AppIndicator
- GnoMenu
- User Themes

Theme:
- Windows-10 (GTK+Shell+Icons) by [@B00merang-Project](https://github.com/B00merang-Project), Licence: GPLv3
- Wallpaper: Aurora (License: [Creative Commons Attribution-ShareAlike 3.0 Unported](https://creativecommons.org/licenses/by-sa/3.0/), Author: [denbol](http://www.panoramio.com/photo/9384842)) 

## macOS

Preview: 
![macOS](http://i.imgur.com/aYAfZxQ.png)

Extensions:
- Dash to dock
- TopIcons Plus
- AppIndicator
- User Themes
- Frippery Move Clock

Theme:
- [Gnome-OSX-II-NT](https://www.gnome-look.org/p/1171688/) (GTK) by [@PAULXFCE](https://www.gnome-look.org/member/455718/), Licence: [Creative Commons](https://creativecommons.org/licenses/by-sa/3.0/) 
- [Human](https://www.gnome-look.org/p/1171095/) (Shell) by [@UMAYANGA](https://www.gnome-look.org/member/434822/) Licence: GPLv3
- [La-Capitaine icons](https://github.com/keeferrourke/la-capitaine-icon-theme) by [@keeferrourke](https://github.com/keeferrourke)


### FAQ: 

#### -My GNOME shell freezes when I run the script.
In some rare occasions your GNOME session might seem to freeze while running the script, however the script is probably still running in the background (you can see the light of your Hard Drive of your computer flashing intensely). Please allow a full minute for the script to complete.

#### -I'm getting various errors on the console while running the script.
This is normal, most of commands are verbose, and some errors occur because you may already have the extensions that the script is trying to download. Please ignore them and allow the script about 1 minute to complete. If the script is interrupted, you can re-run it. When done, close the console, and if you have any issues hit Alt+F2 and type "r" (this will restart X).

#### -Can I save my current layout?
This is currently being worked on.

#### -Any new layouts being added?
A Vanilla GNOME (no extensions) will be added soon, along with the user custom layout. Stay tuned. If you have any ideas, feel free to open an issue or make a pull request.


### Tested on: 
- Manjaro 3.22 X11
- Antergos 3.24 X11
- Fedora 3.22 Wayland (wayland needs to restart after script, and then re-run the script to work) [Preview](http://i.imgur.com/692LOkr.png "Fedora 25 Workstation") 
- Ubuntu 3.24 X11
- Arch Linux 3.24 Wayland

(needs more testing for Wayland)

Licence: GPL 3.0

Author: Bill Mavromatis

Credits: Original extension manager script by Nicolas Bernaerts http://bernaerts.dyndns.org/, United theme by @godlyranchdressing
