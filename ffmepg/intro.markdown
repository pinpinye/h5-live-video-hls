RTMP 协议推流命令:
ffmpeg -re -i /users/pingpingye/Desktop/video/ypp.mp4 -vcodec libx264 -acodec aac -f flv rtmp://127.0.0.1:1935/rtmplive/home
HLS 协议推流命令：
ffmpeg -re -i /users/pingpingye/Desktop/video/ypp.mp4 -vcodec libx264 -vprofile baseline -acodec aac -ar 44100 -strict -2 -ac 1 -f flv -q 10 rtmp://127.0.0.1:1935/hls/test
