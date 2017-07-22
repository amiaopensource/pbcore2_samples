These XML files were made by running http://samples.ffmpeg.org/Matroska/vorbis-audio-switch.mkv through mediainfo, exiftool, and ffprobe.

These commands were used:

```
exiftool -X vorbis-audio-switch.mkv > vorbis-audio-switch.mkv_exiftool.xml
```
```
fits -i vorbis-audio-switch.mkv -xc > vorbis-audio-switch.mkv_fits.xml
```
```
ffprobe -i vorbis-audio-switch.mkv -show_format -show_streams -show_versions -show_chapters -of xml=q=1:x=1 -noprivate > vorbis-audio-switch.mkv_ffprobe.xml
```
```
mediainfo -f --language=raw --output=XML vorbis-audio-switch.mkv > vorbis-audio-switch.mkv_mediainfo.xml
```
