# Other

## How to compress .mov files to .mp4

This is very useful after having recorded your screen with Quicktime.
Compressing to .mp4 will greatly reduce the size of your files.

First, install ffmpeg:

```shell
brew install ffmpeg
```

Then in the directory where your .mov files are stored, run:

```shell
find . -name "*.mov" -print -exec ffmpeg -n -i {} {}.mp4 \;
```
