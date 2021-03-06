# Lofi video wallpaper.

A simple video wallpaper script written in bash using **[mpv](https://mpv.io/)** & **[xwinwrap](https://aur.archlinux.org/packages/xwinwrap-git/)**. Includes audio....

![alt text](https://github.com/furycd001/lofi-video-wallpaper/blob/1b6672e6543dac33193dd2f592d4618f0e2646d5/Screenshot_2021-08-11_20-49-58.png "lofi")

#### How-to install.

1. Download the script....
    ```bash
    wget https://raw.githubusercontent.com/furycd001/lofi-video-wallpaper/main/lofi.sh
    ```
    
2. Open `~/.config/mpv/mpv.conf` & add the following....
    ```bash
    [lofi]
    fullscreen=yes
    title=vwall
    geometry=100%x100%
    border=no
    no-window-dragging
    x11-name=mpv-wallpaper
    hwdec=vaapi
    aid=no
    vo=gpu
    loop-file=no
    shuffle=yes
    loop-playlist=yes
    idle=no
    aid=no
    background="#e5b680"
    panscan=1.0
    ```
> You can remove the bottom line `panscan=1.0` if you do not want the video to fill the screen & be partially cut off.

3. Run the script....
    ```bash
    ./lofi.sh
    ```
4. Enjoy-!!

**OPTIONAL STEPS**
+ Remove audio....
    ```bash
    mpv --no-video https://www.youtube.com/watch?v=5qap5aO4i9A
     ```
> Simply delete this line from the bottom of `lofi.sh` to remove the audio.

+ Change the video to anything you like....
> Simple change the both youtube urls. The first url is for the video wallpaper & the second for the audio.
