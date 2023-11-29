# Welcome to Dotfiles!

Hello there. Welcome to my repository. Here is my updated and fixed Hyprland .config files.


# How to install?

First, update your system using

    sudo pacman -Syyu

That should update the whole Arch Linux system that you got.

Now, install the dependencies

    yay -S base-devel pokemon-colorscripts-git hyprland-git hyprpicker-git xdg-desktop-portal-hyprland-git waybar cava kitty wofi starship wl-clipboard swaync swaylock-effects-git swaylockd tty-clock-git playerctl pavucontrol btop mpd mpd-mpris mpv mpv-mpris qt5-base qt5-wayland qt6-base qt6-wayland lsd geany bat cliphist-bin gamemode polkit-gnome wlogout visual-studio-code-bin boo-grub-git sddm-git boo-sddm-git yad blueman network-manager-applet libinput-gestures light --needed

This should be all.

## GTK Themes, Icons and Cursors

For installing the themes, icons and cursors, you should follow these steps
	
	GTK Theme
	
    cd ~/Downloads
    git clone https://github.com/Fausto-Korpsvart/Tokyo-Night-GTK-Theme.git
    cd Tokyo-Night-GTK-Theme/
    sudo cp -r themes/Tokyonight-Dark-BL-LB /usr/share/themes/
>
    Icons
    
    cd ~/Downloads
    git clone https://github.com/Fausto-Korpsvart/Tokyo-Night-GTK-Theme.git
    cd Tokyo-Night-GTK-Theme/
    sudo cp -r icons/Tokyonight-Moon /usr/share/icons/
>

    Cursors
    cd ~/Downloads
    git clone https://github.com/EliverLara/Sweet.git -b nova
    cd Sweet/
    sudo cp -r kde/cursors/Sweet-cursors /usr/share/icons/

## Config files

For installing the .config files itself, you should follow this steps

    cd ~/Downloads
    git clone https://github.com/kegri/dotfiles
    cd dotfiles
    cp -r .config .icons .local .mpd .ncmpcpp .scripts ~/
    cp .face .fonts.conf .dmrc .gtkrc-2.0 ~/
    chmod -R +x ~/.scripts/
    chmod +x ~/.config/hypr/autostart
    chmod -R +x ~/.config/wlogout/

## Uninstalling

Uninstall your whole system :> (Seriously, I can't think any way that you can uninstall these.)

### Thanks

Without PROxZIMA, this repo would be not exist. So thanks for their work for making this happen. So check them out.
