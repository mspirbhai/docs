https://superuser.com/questions/215430/would-like-to-change-audio-codec-but-keep-video-settings-with-ffmpeg

works perfectly:

```
ffmpeg -i input.avi -acodec mp3 -vcodec copy out.avi
```

Other options:

Just change the audio codec to mp3 (what ever the original codec was)
```
ffmpeg -i input.avi -vcodec copy -acodec mp3 out.avi
```
Just change the video codec to h264
```
ffmpeg -i input.avi -vcodec h264 out.avi
```
no idea just logging
```
ffmpeg -i test.avi -i normalized.mp3 -map 0:0 -map 1:0 -vcodec copy -acodec copy new_test.avi
```


USerd prores and it works, files are bigger but editting is easy
