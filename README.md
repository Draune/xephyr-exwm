# xephyr-exwm

I use EXWM inside Xephyr in KDE Plasma so I don't need to worry about network, bleutooth, sound, and all other things one would wants in is DE.

You must use a X11 WM or DE and not on Wayland (I use KDE Plasma X11) because launching apps from Emacs will open windows outside of it.

You just need to clone the repo and move the files to the correct place.

``` sh
mv exwm.desktop ~/.local/share/applications/
sudo mv xephyr-exwm /usr/bin
```

The following line in `xephyr-exwm` is to be able to use french keyboard:

``` sh
DISPLAY=:2 setxkbmap fr -variant oss
```
