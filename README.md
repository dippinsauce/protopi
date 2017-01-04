# protopi
Files, changes, procedures used to setup RPi 3B used for testing

Used PiBakery to setup image.
Setup Wifi to 'webb2'
Setup VNC to launch on all boot up.

**Needed to change screen default size**
Edited /boot/config.txt
Uncommented the following lines
framebuffer_width=1280
framebuffer_height=720

Needed to change authentication for the vnc server... Had to install RealVNC to connect first time.
Changed VNC -> Options -> Security -> Authentication to "VNC Password"
Set a new password....  Then TightVNC would connect and authenticate.
This allows portable installations to connect via ssh tunnel
