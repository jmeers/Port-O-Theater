# PortableTheater
A Project for an portable mini entertaiment system using a Raspberry Pi

#Goals
- A system that can plug up to a TV using HDMI connection
- Holds 1-2TB of media
- Compact and has a single power plug
- Able to play .mkv files

#Build List
- Raspberry Pi 2 Model B
- Wall charger of at least 2 Amps
- SD Card with OpenELEC installed*
- Portal External hardrive*

*Size depends on need of storage, OpenELEC states >= 2 GB, 4-16 GB is recommended for SD Card.

#Instructions
##Operating System
[Download the OpenELEC OS](http://openelec.tv/get-openelec.)

##USB Power
Once installed on the SD card you will need to edit the config.txt 
Open up the partition that you installed the above Operating system on and look for a file called config.txt and open it.
At the very bottom of the file added `max_usb_current=1`.<br>
The USB ports for the Pi are set by default to 600mA but placing a "1" you make it 1200mA. This will be enough to run your portable harddrive. If for any reason you want it back you can remove the text or change the "1" to a "0". If you have problems with the drive still working then you need to look at your cord it needs to be >=2 Amps because this mod pulls an extra 0.6A of current.

##
