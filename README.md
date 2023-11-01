# THEREMAX 
### A Max4Live controler based on theremin

This project is based on Open.Theremin.UNO 
It requires an Arduino and the Open Theremin hardware.
The open.theremin.uno software has been modified to output pitch value through the serial port. 
The theremax m4l device then reads the values in the serial port and maps it to any audio effect of your choice.

Some elements of the mapper are based on  : http://maxforlive.com/library/device/1791/multimapper

Trouble shooting:
On windows: You may experience errors with stringFormat.js not found. In this case, put stringFormat.js in Max8/Library folder (or any other folder path known by Max > Options > File Preference)

To use the device:
1. Flash the Theremin UNO with the firmware .ino in this repo (not the one from the original OpenThereminUno Archive)
2. Calibrate the Theremin Uno
3. Connect it to your computer using usb cable
4. Add the Theremax device as audio effect to your live set
5. Refresh the Device Finder and select the appropriate Device corresponding to Arduino Theremin
6. Click on the cross on the lower left side to trigger the flow of the serial port read.
7. Calibrate from far away (get away from the theremin and click Calibrate Far)
8. Calibrate from close  (Put your hand close to the theremin and click Calibrate Close)
9. Map the input values audio effect 
10. Adjust the slope for more progressive changes


# OPEN THEREMIN DOC:

## Open.Theremin.UNO control software 

Arduino UNO Software for the Open.Theremin.UNO

### Don't click on the files!
Click on the "Download ZIP" Button to the right or [Click here](https://github.com/GaudiLabs/OpenThereminUNO/archive/master.zip) 
Then unpack the archive.

### Open Source Theremin based on the Arduino Platform

Open.Theremin.UNO is an arduino shield to build the legendary music instrument invented by Leon Theremin back in 1920. The theremin is played with two antennas, one to control the pitch and one for volume. The electronic shield with two ports to connect those antennas comprises two heterodyne oscillators to measure the distance of the hand to the antenna when playing the instrument. The resulting signal is fed into the arduino. After linearization and filtering the arduino generates the instruments sound that is then played through a high quality digital analog audio converter on the board. The characteristics of the sound can be determined by a wave table on the arduino.

For more info on the open source project and on availability of ready made shield see:

http://www.gaudi.ch/OpenTheremin/

### Installation
1. Open up the Arduino IDE
2. Open the File "Open_Theremin_UNO.ino"
3. Selecting the correct usb port on Tools -> Serial Port
4. Select the correct arduino board from Tools -> Board
5. Upload the code by clicking on the upload button.

