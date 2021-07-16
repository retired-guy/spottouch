# spottouch
RPi Touchscreen Remote Control for Spotify

Tested on RPi Zero WH with Hyperpixel 4" touchscreen display

You'll need a Spotify developer account, and will need to add SPOTIPY_CLIENT_ID, SPOTIPY_CLIENT_SECRET and SPOTIPY_REDIRECT_URI environment variables.  I export them in a bash script which starts the python script.  https://spotipy.readthedocs.io/en/2.18.0/

In order to run as the pi user to access the framebuffer, you'll need to add it to the video group:

usermod -a -G video pi
