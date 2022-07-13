Chrome will not detect the input device unless running with exlusive caps mode
sudo modprobe v4l2loopback devices=1 exclusive_caps=1

The device will not be visible within Chrome unless there is media flowing
ffmpeg -stream_loop -1 -re -i vid1.mov -f v4l2 /dev/video0

The scanner library require https to serve the content therefore run
python3 httpssrv.py

