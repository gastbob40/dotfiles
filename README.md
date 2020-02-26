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

6. **Install `feh` to use background images.**
```bash
sudo pacman -S feh
```

7. **Install I3 manager.** I personally choose a fork of this version, `i3-gaps`. You can find my file configuration in the config folder.
```bash
sudo yay -S i3-gaps
```

8. **Install [Polybar](https://github.com/polybar/polybar/wiki).** My configuration file can be found in the config folder.
```bash
sudo yay -S polybar
mkdir .config/polybar
touch .config/polybar/config
yay -S ttf-font-awesome-4
```

9. **Install `rofi`, a run command interface.** My configuration file can be found in the config folder.
```bash
sudo pacman -S rofi
```

10. **Add a composite manager, as [Picom](https://wiki.archlinux.org/index.php/Picom).**
```bash
sudo pacman -S picom
mkdir ~/.config/picom/
cp /etc/xdg/picom.conf ~/.config/picom/picom.conf
picom --config ~/.config/picom/picom.conf
```

11. **Install a new bash, as [Fish](https://wiki.archlinux.org/index.php/Fish). You can also install [Oh My Fish](https://github.com/oh-my-fish/oh-my-fish).** You can find some fish's themes [here](https://github.com/oh-my-fish/oh-my-fish/blob/master/docs/Themes.md). 
```bash
sudo pacman -S fish
chsh -s /usr/bin/fish
curl -L https://get.oh-my.fish | fish
omf install robbyrussell
omf theme robbyrussell
set -U fish_greeting ""
```

