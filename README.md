# video2stream
using the power of videojs and ffmpeg we take a video, convert it, and stream it

# usage
```
video2stream [filename]
```

This creates the following structure:

[filename].html: An html file that loads the video in a browser

[filename]-video: A folder containing the m3u8 playlist and all the necessary .ts files

[filename]-video/md5.m3u8: The playlist, which is named after the first 9 digits of the md5 of the source video

[filename]-video/md5-dataxxxx.ts: .ts video segments of the streamed video
