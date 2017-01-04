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

Needed to change authentication for the vnc server... Had to install RealVNC to connect first time.  
Changed VNC -> Options -> Security -> Authentication to "VNC Password"  
Set a new password....  Then TightVNC would connect and authenticate.  
This allows portable installations to connect via ssh tunnel  

Setup pi to boot from attached usb drive...  
Following instructions found https://github.com/raspberrypi/documentation/blob/master/hardware/raspberrypi/bootmodes/msd.md  

Next Steps -- Install utilities to work the 433MHz receiver and capture signals...  
