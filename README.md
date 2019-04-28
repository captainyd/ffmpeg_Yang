# ffmpeg_Yang
command notes

## extract frames from a video
  ffmpeg -i video.mp4 -q:v 2 -vf fps=1 -start_number 0 -ss 00:00：00 -t 10 outpath/%04d.jpg

## convert images to a video
  ffmpeg -r 60 -f image2 -s 1920x1080 -i pic%04d.png -vcodec libx264 -crf 25  -pix_fmt yuv420p test.mp4
