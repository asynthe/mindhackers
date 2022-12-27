
# FFmpeg
---
[main page](https://ffmpeg.org/)
[arch wiki](https://wiki.archlinux.org/title/FFmpeg)
[foss - ffmpeg guide](https://itsfoss.com/ffmpeg/)

arch ->
gentoo -> `media-video/ffmpeg`

__RECORDING VIDEO + AUDIO__
[main page - capturing your desktop](https://trac.ffmpeg.org/wiki/Capture/Desktop)

### __RECORDING VIDEO__
https://ubunlog.com/en/graba-tu-escritorio-desde-el-terminal-con-ffmpeg/

### __RECORDING AUDIO__
note: remember to have your desired sound architecture flag compiled in Gentoo's FFmpeg (`pulseaudio`, `alsa`)

first, check your devices name
```
$ pactl list short sources
```

example:
```
49	alsa_input.usb-Razer_Inc_Razer_Seiren_Mini_UC2216L03206474-00.mono-fallback	PipeWire	s16le 1ch 48000Hz	RUNNING
145	alsa_output.pci-0000_00_1f.3.analog-stereo.monitor	PipeWire	s32le 2ch 48000Hz	RUNNING
```

in this case, i want to record my Razer Seiren Mini, so i can do both:
```
$ ffmpeg -f pulse <input_options> -i 49 output.wav
or
$ ffmpeg -f pulse <input_options> -i alsa_input.usb-Razer_Inc_Razer_Seiren_Mini_UC2216L03206474-00.mono-fallback output.wav
```


you can also record your Desktop and use the [[listen script]], to hear your own voice an

__RECORDING IN YOUR LINUX DESKTOP__
__X11__

__WAYLAND__



### __CONVERTING__
easy way
```
$ ffmpeg -i input.mp4 output.avi
```

https://www.bannerbear.com/blog/how-to-make-a-gif-from-a-video-using-ffmpeg/

### __CUTTING__
cutting audio from a video with ffmpeg
https://stackoverflow.com/questions/38161697/how-to-remove-one-track-from-video-file-using-ffmpeg

https://shotstack.io/learn/use-ffmpeg-to-trim-video/

### __COMPRESSING__
$ 
