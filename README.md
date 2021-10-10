# How to Shoot Time-Lapse Videos with a USB-Camera


## How to use this script
1. Make sure that the folder `/home/pi/Pictures` and `/home/pi/Videos` is created
2. Adapt the `webcam.cfg` according to your needs (*You can find the possible resolution and webcam controls with the following commands*)
3. Adapt the `timelapse.py` parameters (duration, resolutions, fps)
3. You can run the script with `python3 timelapse.py`

### If you want to use screen
Start the script: `screen -dmLS timelapse python3 timelapse.py`
Reattach to the session with: `screen -r timelapse`
Exit the session by pressing `CTRL+A` following by `CTRL+R` 


### List possible webcam output resolutions
`v4l2-ctl -d /dev/video0 --list-formats-ext`


### List possible webcam controls
`fswebcam --list-controls`
