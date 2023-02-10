## suckless terminal (perfect + colors using xresources)

## Install

```
wget https://raw.githubusercontent.com/Ahwxorg/st/main/.Xresources ~/.config/Xresources
git clone https://github.com/ahwxorg/st
cd st
sudo make clean install
xrdb merge ~/.config/Xresources
```

(note : put the xrdb merge command in your wm's autostart or similar) 

## Fonts 

- Install JetbrainsMono Mono Nerd Font [here](https://www.nerdfonts.com/font-downloads).

## Patches:

- Ligatures
- sixel (check sixel branch)
- scrollback
- Clipboard
- Alpha(Transparency)
- Boxdraw
- patch_column
- font2
- right click paste
- st desktop entry
- newterm
- anygeometry
- xresources
- sync patch
- live reload
- default font size

## Alias for live reload

```
alias rel="xrdb merge ~/.Xresources && kill -USR1 $(pidof st)"
```

## Default keybindings

```
ctrl + shift + c        copy
ctrl + shift + v        paste + right click on the terminal will paste the clipboard

zoom
alt  + comma            zoom in
alt  + .                zoom out
alt  + g                reset zoom

transparency
alt  + s                increase transparency
alt  + a                decrease transparency
alt  + m                reset transparency

alt + k                 scroll down
alt + j                 scroll up

mod + shift + enter    open a new terminal with same working directory
```

You can change all of these in config.h

## Credits

- [ls-icons](https://github.com/Yash-Handa/logo-ls)
- JetbrainsMono Nerd Font + material design icon font.
- [Siduck/st](https://github.com/siduck/st): for 99% of this build.
- [live-reload](https://github.com/nimaipatel/st) 
- [patch_column](https://github.com/nimaipatel/st/blob/all/patches/7672445bab01cb4e861651dc540566ac22e25812.diff)
