# Opera

## OPERA VIDEO PLAY

Some types of videos and Lives not playing correctly or not playing at all.
What you need to do is:

### Install 'snap'
[To install snap I have done a tutorial here](../snap/README.md)

### Install chromium ffmpeg
To install ffmpeg do:

```sh
sudo apt update && sudo snap install chromium-ffmpeg
```

### Create a symlink
An easy way to understand a symlink is like a shortcut to an archive, but the system really believes the archive is in there. I don't go in deep in this topic now.

First step is to create a directory named as lib_extra inside opera dir path.

```sh
sudo mkdir /usr/lib/x86_64-linux-gnu/opera/lib_extra
```

After this you gona really create the symlink:

```sh
sudo cp /snap/chromium-ffmpeg/current/chromium-ffmpeg-104195/chromium-ffmpeg/libffmpeg.so /usr/lib/x86_64-linux-gnu/opera/lib_extra
sudo cp /opt/google/chrome/WidevineCdm/_platform_specific/linux_x64/libwidevinecdm.so /opt/google/chrome/libwidevinecdm.so

```

You really need to check if the directory chromium-ffmpeg-98516 is inside /snap/chromium-ffmpeg/current/ to make sure that is working.

#### !!! NOW RESTART OPERA !!!

### Final
And now if you done everything correctly the Opera maybe show the videos and lives from TWITCH, YOUTUBE and other platforms nicely.
