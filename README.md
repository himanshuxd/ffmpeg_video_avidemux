# ffmpeg_video_avidemux
Various tools and commands for video editing and cropping.

# cropping a video
    ffmpeg -i in.mp4 -filter:v "crop=W_:H_:W_:H_"   Vid-out.mp4

# splitting a mp4 file
    ffmpeg -i ORIGINALFILE.mp4 -acodec copy -vcodec copy -ss START -t LENGTH OUTFILE.mp4

# loop a video file into .mkv format
    ffmpeg -i input.mp4 -c copy output.mkv

# loop a video file to .mp4 format
    ffmpeg -stream_loop 4 -i output.mkv -c copy output.mp4
