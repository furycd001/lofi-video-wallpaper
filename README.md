# Lofi video wallpaper.

A simple video wallpaper script written in bash using **[mpv](https://mpv.io/)** & **[xwinwrap](https://aur.archlinux.org/packages/xwinwrap-git/)**. Includes audio. Inspired by **[this post](https://www.reddit.com/r/unixporn/comments/p292xv/oc_i_made_a_script_that_plays_the_lofi_stream_in/?utm_source=share&utm_medium=web2x&context=3)** made by **[u/rapphyyy](https://www.reddit.com/user/rapphyyy/)**.

#### How-to install.

1. Download the script....
    ```bash
    wget https://raw.githubusercontent.com/furycd001/dots/master/Gucci/lofi.sh
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

5. Optional step to remove audio....
	 ```bash
	mpv --no-video https://www.youtube.com/watch?v=5qap5aO4i9A
	 ```
> Simply delete this line from the bottom of `lofi.sh` to remove the audio.
