# protopi
Files, changes, procedures used to setup RPi 3B used for testing  

Used PiBakery to setup image.  
Setup Wifi to 'webb2'  
Setup VNC to launch on all boot up.  
ssh left at default port of 22, router will handle the external port routing.  

**Needed to change screen default size for VNC**  
Edited /boot/config.txt  
Uncommented the following lines  
framebuffer_width=1280  
framebuffer_height=720  

Didn't perform these steps, installed RealVNC to my portable drive.  
_Needed to change authentication for the vnc server... Had to install RealVNC to connect first time.  
_Changed VNC -> Options -> Security -> Authentication to "VNC Password"  
_Set a new password....  Then TightVNC would connect and authenticate.  
_This allows portable installations to connect via ssh tunnel  

Setup pi to boot from attached usb drive...  
Following instructions found https://github.com/raspberrypi/documentation/blob/master/hardware/raspberrypi/bootmodes/msd.md  
This didn't work at all... Tried with the corsair 32gb SSD in the sabrent enclosure through the Ankey portable USB3 hub.
Starting from scratch.  Just gonna run on the sd card.  

Next Steps -- Install utilities to work the 433MHz receiver and capture signals...  
