# xde-menu-compilation
Instructions for compiling xde-menu on Debian like distros.
### Install libraries:

autoconf autogen automake libtool

libgnome-menu-3-dev libwnck-dev libgtk2.0-dev libgdk-pixbuf2.0-dev libx11-dev libxext-dev libice-dev libsm-dev

### Additional

murrine-themes

### Use

in file /etc/apt/apt.conf.d/99-update-menus

DPkg::Post-Invoke {"xde-menu --menugen --wmname=icewm --format=icewm --root-menu /etc/xdg/menus/lxde-applications.menu --nolaunch --output /usr/share/icewm/menu";};

Change /etc/xdg/menus/lxde-applications.menu by your instaled menus
