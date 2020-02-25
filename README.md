# DotFiles and Manjaro Installation

## About

This project is mainly for personal use, and allows me to easily create a new machine running on manjaro. It contains:

- My commands for manjaro installation
- My configuration files for my different applications

## Getting started

1. **Installing manjaro through its [website](https://manjaro.org/download/).** I personally choose XFCE.

2. **Configure pacman mirrors, to get the faster.**
```bash
sudo pacman-mirrors --fasttrack
```

3. **Update all Manjaro package.** Remember to restart the PC afterwards.
```bash
sudo pacman -Syyu
```
4. **Install Yay to get access to AUR.**
```bash
git clone https://aur.archlinux.org/yay.git
cd yay
makepkg -si
```

5. **Install a login manager screen, as [LightDM WebKit2](https://github.com/Litarvan/lightdm-webkit-theme-litarvan).**

6. **Install I3 manager.** I personally choose a fork of this version, `i3-gaps`. You can find my file configuration in the config folder.
```bash
sudo yay -S i3-gaps
``` 

7. **Install `rofi`, a run command interface.** My configuration file can be found in the config folder.
```bash
sudo pacman -S rofi
```

8. **Add a composite manager, as [Picom](https://wiki.archlinux.org/index.php/Picom).**
```bash
sudo pacman -S picom
mkdir ~/.config/picom/
cp /etc/xdg/picom.conf. ~/.config/picom/picom.conf
picom ~/.config/picom/picom.conf
```