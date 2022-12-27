---
title: "guides"
---

# Guides ガイド
---

### What I Study お勉強

A Guide to [FILESYSTEMS]({{< ref "a_guide_to/FILESYSTEMS/FILESYSTEMS.md" >}})
{{< line_break >}}
A Guide to [BACKUPS]({{< ref "a_guide_to/BACKUPS/BACKUPS.md" >}})
{{< line_break >}}
A Guide to [VIRTUAL MACHINES]({{< ref "a_guide_to/VIRTUAL_MACHINES/VIRTUAL_MACHINES.md" >}})
{{< line_break >}}
A Guide to [CONTAINERS]({{< ref "a_guide_to/CONTAINERS/CONTAINERS.md" >}})
{{< line_break >}}
A Guide to [VERSION CONTROL]({{< ref "a_guide_to/VERSION_CONTROL/VERSION_CONTROL.md" >}})
{{< line_break >}}
A Guide to [SSH]({{< ref "a_guide_to/SSH/SSH.md" >}})
{{< line_break >}}
A Guide to [MONERO]({{< ref "a_guide_to/CRYPTO/CRYPTO.md" >}})
{{< line_break >}}
{{< line_break >}}


A Guide to NETWORKING]({{< ref "a_guide_to/CONTAINERS/CONTAINERS.md" >}})
{{< line_break >}}

Static websites with [[Hugo]]
{{< line_break >}}
Presentations with [[Marp]]
{{< line_break >}}
Professional Docs with [[LaTeX]
]{{< line_break >}}

VIDEO / Audio with FFmpeg

---


file database finder -> [[locate]]
[[xdg-utils]]

[dracut options](https://manpages.ubuntu.com/manpages/bionic/man7/dracut.cmdline.7.html)

net-misc/ntp for time and hwclock

-> __general__
- what i use specified through my [[mimeapps.list]] list
- downloading youtube videos with [[yt-dlp]]
- synched folders across devices using [[Syncthing]]
- setting mp4 wallpapers with [[wallset]]
- filtering blue color at night with [[redshift]] (X11) / x (Wayland)
-> writing in japanese with 
- [[ibus-anthy]] (gentoo)
- [[fcitx5-mozc]] (arch)

-> __backups__
- [[Rustic]]
- [[Borg]]

rsync + cron
syncthing
-> __backup through apps__ -


-> __video__
- recording video with [[system/dotfiles/utils/FFmpeg]]
- take screenshots with [[system/dotfiles/ImageMagick]]
-> __audio__
- installing [[Pipewire]]
- recording audio with [[system/dotfiles/utils/FFmpeg]]
- show microphone audio in [[cli-visualizer]]
- listen to your own mic with the [[listen script]]

-> __extra__
- unclutter your home folder with [[xdg-ninja]]
- listening to the [[soul of the kernel]]
- [[system/dotfiles/quotes]] for zsh

__tools__
-> version control using [[git 1]]
-> split terminal sessions with [[tmux]]
-> compress files with 
[[zip]] / [[7zip]] / [[rar]] / [[gzip]] / [[tar]]
-> record the screen using [[system/dotfiles/utils/FFmpeg]]
-> convert images through [[system/dotfiles/ImageMagick]]

__system__
-> [[automounting windows partition]]

-> changing the default [[dns]]
-> set up [[system/dotfiles/default applications]]
-> making custom linux [[desktop]] files to use as default apps
-> setting up local database with [[locate]]
- set up time automatically with [[ntp]]
- -> [[using hard links and soft links]]
-> [[little chmod guide]]
-> cat, grep and [[sed]]
-> how many system resources your user can usue with [[ulimit]]

__fixes__
-> [[strange noise in headphones]] when no sound is played

[chmod command - linuxize](https://linuxize.com/post/chmod-command-in-linux/)

-> see which keys are pressed and registered with

```bash
$ showkey -a
```

-> extracting a tar file

for the .zip files you can use unzip
>$ unzip [archive.zip]

for .tar.xz you can use tar (comes with most of linux distros)
>$ tar -xf [archive.tar.xz]
>$ x (--extract) -> extract
>$ f -> 


-> disabling the PC speaker (for that loud beep)
[arch wiki](https://wiki.archlinux.org/title/PC_speaker#Disabling_the_PC_speaker)


# ricing
---
GRUB -> grub-customizer
rEFInd -> [rEFInd-minimal](https://github.com/evanpurkhiser/rEFInd-minimal) / [rEFInd-minimal-dark](https://github.com/Kissycat/rEFInd-minimal-dark)

**Distro Themes**
XFCE -> [Chicago95](https://github.com/grassmunk/Chicago95/)
Ubuntu -> [Moebuntu](http://moebuntu.web.fc2.com/home_eng.html)

add user to group
```
# usermod -a -G <group> <user>
```
