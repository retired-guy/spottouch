# spottouch
RPi Touchscreen Remote Control for Spotify

Tested on RPi Zero WH with Hyperpixel 4" touchscreen display

You'll need a Spotify developer account, and will need to add SPOTIPY_CLIENT_ID, SPOTIPY_CLIENT_SECRET and SPOTIPY_REDIRECT_URI environment variables.  I export them in a bash script which starts the python script:  https://spotipy.readthedocs.io/en/2.18.0/

In order to run as the pi user to access the framebuffer, you'll need to add it to the video group:

usermod -a -G video pi

To start this at boot, create a service file and launch the bash script with it:
https://www.raspberrypi.org/documentation/linux/usage/systemd.md

![photo](https://1.bp.blogspot.com/-upQ2l_DWhIM/YPDlRrgvhaI/AAAAAAAAulI/UFjkNtX9se8dsge0MW4NBAE2EpagwneuwCLcBGAsYHQ/s1333/In_Action.jpeg)
