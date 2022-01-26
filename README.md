# CJMCU_ATMEGA32U4_BADUSB
The CJMCU clones of the RubberDucky are no different when it comes to be used by pentesters but it surely has a different circuit mesh to get around as a new user of this device; There are many ways to flash the firmware or inject payloads when it comes to rubber duckies and badusbs but unfortunately you'll end up wasting your time downloading numerous exploits and firmware flash tools and to no help given so in this repo i will be showing how to upload a rubber ducky script along with the arduino code to make it work.
Things you will need:
1.ATMEGA32U4 Arduino Ducky By CJMCU with SD card support.
2.Arduino IDE (https://www.arduino.cc/en/Main/Software)
3.An SD Card and a SD card reader
4.No soldering needed

![cjmcu-virtual-keyboard-badusb-usb-ttf-memory-keyboard-atmega32u4-module jpg_640x640](https://user-images.githubusercontent.com/34340232/43675104-39aa9d88-97e7-11e8-884b-608997c0bbbb.jpg)


#Notice the SD Card Slot#

the Atmega32u4 By CJMCU has a memory slot for intaking any sort of good quality SD cards where the formatting should be FAT32 and can be of any limit i myself am using the MicroSD by Kingston 16GB also you will need an SD card reader or an Adapter thats comes with a newly purchased SD card.

#How to upload the Arduino script#

Before you upload the script you need to 'Tell' your BADUSB to use the SD card slot, now in order to do that you will need to Upload an Aduino script .ino which will tell the USB to read the SD slot which you can download from here (https://github.com/Seytonic/Duckduino-microSD/blob/master/Duckduino-microSD/Duckduino-microSD.ino) the Script is made by https://github.com/Seytonic 
upload the .ino script to your BADUSB and when it is successful the BADUSB will flash a red LED to confirm the upload.

#Uploading the ducky script#

Now you may first plug in your SD card into the card reader and download the ducky script of your choice from here (https://github.com/hak5darren/USB-Rubber-Ducky/wiki/Payloads) made by (https://github.com/hak5darren) 
Name your desired script as 'script' as a textfile in the SD card(some may require you to make your own changes in order for them to work start with the easy one as a kickstarter with 'Hello world') since the .ino code tells the USB to read the ducky script file with the name 'script'.

#The Final Work#

Now that the script is in the SD card plug the SD Card into the USB and then plug the USB into the computer and see the magic.

