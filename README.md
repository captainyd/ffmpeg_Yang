# ffmpeg_Yang
command notes
## extract frames from video
'''
ffmpeg -i video.mp4 -q:v 2 -vf fps=1 -start_number 0 -ss 00:00：00 -t 10 outpath/%04d.jpg
'''
