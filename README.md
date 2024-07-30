# CamillaDSP-Implemantation
Implementing CamillaDSP on a Raspberry Pi 5 on a 10.1" Touch screen

Here is a photo of the touch screen showing CamillaDSP (CDSP) with JiveLite.
![alt text](<Images/10.1 screen front on shelf.jpg>)

This photo shows the back of the screen with the RPi5 mounted. The support legs have a slot  allowing cables to be fed through keeping some tideness. The FLIRC is attached on the right hand side to a USB extension cable, the old Squeezebox remote is beside the screen.
![alt text](<Images/10.1 back showing RPi5 plugs and FLIRC and remote.jpg>)

This is a Prt Sc from the RPi5 showing the screen in more detail while playing.
Note the top row of the screen showing icons, on the left the Raspberry will display a drop down menu for various system utilities, the keyboard will display/hide the on-screen keyboard. The icons on the far right also show details in drop down menus. The CDSP volume can be altered either by the slider or with the remote. The JiveLite screen will be familiar to Squeezebox (LMS) users.
![alt text](<Images/10.1 screen Jivelite and Firefox CamillaDSP.jpg>)

This Prt Sc shows the CDSP Devices tab with the on-screen keyboard.
 ![alt text](<Images/10.1 screen Devices tab with on-screen keyboard.jpg>)

This Prt Sc shows the CDSP File tab. 
![alt text](<Images/10.1 screen CamillaDSP Files tab.jpg>)

This Prt Sc shows the Pipeline in collapsed mode.
![alt text](<Images/10.1 screen Pipeline - collapsed.jpg>)
 

Following https://www.audiosciencereview.com/forum/index.php?threads/rpi-camilladsp-tutorial.29656/ I built CamillaDSP running on a Raspberry Pi 5 to tri-amp a pair of modified Klipschorns, a USB connected Motu UltraLite Mk.5 provides the balanced analog output to the three stereo amplifiers.

Initially I ran Squeezelite on the Raspberry Pi with CamillaDSP and controlled it via a  PiCorePlayer on another Raspberry Pi running on a 7" screen. I then tried installing and running JiveLite on the RPi 5 with CamillaDSP instead of SqueezeLite and attached a 7" touch screen. As well as the streaming facility, JiveLite provides player controls and display. This worked fairly well, but could be improved with a bit more screen space to avoid swapping from app to app, so I bought a Waveshare 10.1" touch screen with a stand and provision for mounting a RPi on the back. By running the Raspberry Pi desktop OS instead of Raspberry Pi Lite and adding an on-screen keyboard there is now full control of the internet browser for CamillaDSP without the need for an attached keyboard. 

Components - 
Raspberry Pi 5 and 32GB SD card.

Waveshare 10.1inch Capacitive Touch Screen LCD (B) with Case 1280×800 HDMI IPS Display Compatible with Raspberry Pi.
https://www.amazon.com.au/Waveshare-10-1inch-Capacitive-Compatible-Raspberry/dp/B0BFQGZ2NV

Software -
CamillaDSP as per the CamillaDSP tutorial.

Jivelite - full install instructions from Man in a van here -
https://forums.slimdevices.com/forum/user-forums/linux-unix/95254-announce-jivelite-cut-down-squeezebox-control-application/page33#post1681857

On-screen keyboard for RPi 5 running Pi OS (Bookworm)
https://forums.raspberrypi.com/viewtopic.php?t=358147
