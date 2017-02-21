#Raspberry Pi Setup

##Installing image on SD card

Get Raspbian Jessie based PiTFT image from:

[https://s3.amazonaws.com/adafruit-raspberry-pi/2016-10-18-pitft-28r.zip](https://s3.amazonaws.com/adafruit-raspberry-pi/2016-10-18-pitft-28r.zip)

Instructions for installing images:

https://www.raspberrypi.org/documentation/installation/installing-images/README.md

##Configuration
Preferences > Raspberry Pi Configuration
System Tab "Expand Filesystem"
The reboot.

##Software
```
sudo apt-get update
sudo apt-get upgrade
```

<!---##Rotate screen
If using with 7" official raspberry pi touch screen, may need to rotate display. To do this, open /boot/config.txt in your favourite editor and add the line:
```
lcd_rotate=2
```

distribution used: Raspbian

configuration

display
--->

