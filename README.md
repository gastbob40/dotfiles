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


