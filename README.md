# CamillaDSP-an-Implemantation
### Implementing CamillaDSP on a Raspberry Pi 5 on a 10.1" Touch screen

Here is a photo of the touch screen showing CamillaDSP (CDSP) with JiveLite.
![alt text](<Images/10.1 screen pi running CDSP & JiveLite.jpg>)
![alt text](<Images/10.1 screen front pic.JPG>)


This photo shows the back of the screen with the RPi5 mounted. The support legs have a slot  allowing cables to be fed through keeping some tideness. The FLIRC is attached on the right hand side to a USB extension cable, the old Squeezebox remote is beside the screen.
![alt text](<Images/10.1 back showing RPi5 plugs and FLIRC and remote.jpg>)
![alt text](<Images/10.1 screen back showing RPi5.JPG>)

Enough photos, I mastered the highly technical process of Print Screen (Prt Sc) on the RPi5 - connect a USB keyboard and press Prt Sc. The resulting screen pic is stored in a folder called Pictures. Who would have thought!

This is a Prt Sc from the RPi5 showing the screen in more detail while playing.
Note the top row of the screen showing icons, on the left the Raspberry will display a drop down menu for various system utilities, the keyboard will display/hide the on-screen keyboard. The icons on the far right also show details in drop down menus. The CDSP volume can be altered either by the slider or with the remote. The JiveLite screen will be familiar to Squeezebox (LMS) users.
![alt text](<Images/10.1 screen Jivelite and Firefox CamillaDSP.jpg>)

This Prt Sc shows the CDSP Devices tab with the on-screen keyboard. The keys are big enough for good typing accuracy with big hands.
![alt text](<Images/10.1 screen Devices tab with on-screen keyboard.jpg>)

This Prt Sc shows the CDSP File tab. 
![alt text](<Images/10.1 screen CamillaDSP Files tab.jpg>)

This Prt Sc shows the Pipeline in collapsed mode.
![alt text](<Images/10.1 screen Pipeline - collapsed.jpg>)

This Prt Sc shows the Shortcuts tab with the Bass and Treble tone control sliders. Similar to the Volume slider these sliders take effect immediately - well, almost immediately, allowing for the delays in processing, 5ms due to time aligning the drivers and then however long the FIR filters delay things. I use these to add a little life (room curve) as the speakers are EQd flat.
![alt text](<Images/10.1 screen CamillaDSP Shortcuts.jpg>)

 This Prt Sc shows the JiveLite screensaver Word Clock. This is the screen saver I use on my PiCorePlayers.
 ![alt text](<Images/10.1 screen JiveLite screensaver Word Clock.jpg>)

Following https://www.audiosciencereview.com/forum/index.php?threads/rpi-camilladsp-tutorial.29656/ I built CamillaDSP running on a Raspberry Pi 5 to tri-amp a pair of modified Klipschorns, a USB connected Motu UltraLite Mk.5 provides the balanced analog output to the three stereo amplifiers.

I have documented the process of building the CamillaDSP config for my K-Horns using REW and rePhase here - https://github.com/wirrunna/CamillaDSP-Building-a-Config . REW will save filters in CamillaDSP compatible format that CamillaDSP can import using the GUI.


Initially I ran CamillaDSP and Squeezelite on a headless Raspberry Pi with the OLED volume display as recommended in Michael's tutorial. The music was controlled via a  PiCorePlayer on another Raspberry Pi running on a 7" screen. 

I then tried installing and running JiveLite on the RPi 5 with CamillaDSP instead of SqueezeLite and mounted the RPi on the back of a 7" touch screen display. As well as the streaming facility, JiveLite provides player controls and display. This worked fairly well, but required swapping from JiveLite to CDSP to see the volume.

After a bit of research I bought a Waveshare 10.1" touch screen with a stand and provision for mounting a RPi on the back (details in the link to Waveshare below). 

By running the Raspberry Pi desktop OS instead of Raspberry Pi Lite and adding an on-screen keyboard there is now full control of the internet browser for CamillaDSP without the need for an attached keyboard. The full suite of RPi software utilities are also available (including Prt Sc). My understanding is that the RPi Desktop does not load software until it is executed and so it doesn't use more RAM than the RPi OS Lite, however it does use a few GB more storage but will safely run on a 32GB SD card. In fact after backup of my SD Card I loaded GParted and shrunk the SD card to 14 GB and have since copied the image onto several different SD cards to prove a theory that an SD image could be copied to Google Drive and downloaded and restored to give a working system.

### Components - 
Raspberry Pi 5 and 32GB SD card.

https://www.waveshare.com/10.1inch-hdmi-lcd-b-with-case.htm

Wave share have a higher resolution screen (1080x1200) in a sexier case but I think the RPi will need a VESA mount and the case is more expensive.

### Software -
CamillaDSP as per the CamillaDSP tutorial.

Jivelite - full install instructions from Man in a van here -
https://forums.slimdevices.com/forum/user-forums/linux-unix/95254-announce-jivelite-cut-down-squeezebox-control-application/page33#post1681857

On-screen keyboard for RPi 5 running Pi OS (Bookworm)
https://forums.raspberrypi.com/viewtopic.php?t=358147

