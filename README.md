# E58-Gimbal-Project
E58 Gimbal Project
https://www.youtube.com/watch?v=9We7zRGdLF4&lc=UgwFp6yRhZ_iBawvzqJ4AaABAg&feature=em-comments
For those that wanted to know how I added the gimbal to the front of the E58 drone.  I take NO responsibility should anything go wrong with your drone.  I’m basically trying to remember what I did a few years ago.  So please understand if something isn’t quite right or you spot an error.

Note recording to the SD will no longer work after this.

What we’re going to attempt to do is repurpose the wire that starts the SD card board recording so that instead of starting and stopping the record function (through the button press on the remote) it now sends the signal to the Arduino Micro which in turn moves the gimbal up or down when pressed.
What we’ll need.
1.	A Dremel or something similar to cut the bottom part off the drone case as seen in the video.
2.	An Ardunio Micro
3.	Some wires to solder it up
4.	A pico servo motor (https://www.espruino.com/Servo+Motors)
5.	3d printed gimbal bracket - .STL attached.

Steps
Notes – check all voltages – micro needs 5v only.
1.	Open the drone up but undoing all the screws.
2.	Take out all the internal boards (2 in essence. Main board and on/off switch and SD card/camera board.
3.	Wire up the micro to the main board power + and ground.
4.	Now the wire that goes to the SD card board that now needs to go to the micro pin 8 and the same wire going to the sd card (yellow)
5.	The servo requires three wires, positive, negative and signal.  
6.	Wire servo + and negative to main board power terminals.
7.	Pin 9 on the micro now goes to the servo
8.	Upload sketch to micro (in this git)
9.	Test.  When the button is pressed the servo should rotate up or down
10.	Glue 3d printed bracket to lower case.
11.	Glue servo to bracket
12.	Screw everything back together – now a tight fit because of the addition of the micro.
