# mediafiles
Example media files for testing

## Enhanced RTMP

Example files for E-RTMP created with FFmpeg

* AV1 `ffmpeg -stream_loop -1 -re -i test.mp4 -c:v libsvtav1 -b:v 1M -c:a aac -b:a 128k -ar 48000 -ac 2 -f flv "rtmp://10.0.0.35:1935/live/streamAV1"`
* VP8 `ffmpeg -stream_loop -1 -re -i test.mp4 -c:v libvpx -b:v 1M -c:a aac -b:a 128k -ar 48000 -ac 2 -f flv "rtmp://10.0.0.35:1935/live/streamVp8"`

More coming soon as the other codecs are implemented. Note that VP8 flv playback requires a patched FFmpeg ffplay (see patch)

