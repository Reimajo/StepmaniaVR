# StepmaniaVR
A Stepmania DDR Dance-Pad emulator using SteamVR with Vive Trackers. This program was made by KeksTheFurry and Tekki 
in only one day with almost zero knowledge about SteamVR and C++.  

See the software in action (together with Stepmania 5):
https://www.youtube.com/watch?v=2mgoQEJnbRI

It uses third party source code from SteamVR, as well as code snippets from various websites (check source code for details). 
We do not claim any of that, do whatever you want with it. This source code is very ugly and we are aware of that, but it works. 

We hope that someone adds a UI in the future for usability. The only purpose of this program was to have a proof-of-concept 
that this is possible and works with Stepmania. This tool requieres Steam VR being up and running before you start it. 
You need 2 Vive Trackers on your feet or on your legs (the trackers being on your ancles & facing forward is recommended). 

You should have a 3 x 3 tile area with 30cm x 30cm tiles which acts as your Stepmania dancepad (does not need to exists 
IRL but it is recommended to put markers on the floor for your own reference). You need at least 2 corners (top right and 
bottom left, e.g. 134cm apart) for calibration. The distance varies the total size of your dance pad. It is recommended 
to have the middle pile out of a material that you can feel under your feet, e.g. a cardboard cutout with double-tape 
on the bottom to stick to the floor. 

After startup of this program, you have 10 seconds to stay front-facing on your two calibration points 
(trackers must be right over your calibration points). This program does not calculate any offset for your feet, it uses 
the raw tracker position for everything! As soon as StepMania is being started, the calibration is finished and you should 
be able to play. If you start the program from within visual studio, you will be able to see the debug logs which is helpful. 
Else just download the StepmaniaVR folder from Github and run the StemaniaVR.exe from within that folder.

The sourcecode can be found in github under /StepmaniaVR/sourcecode/samples/
Just open this file in Visual Studio: /StepmaniaVR/sourcecode/samples/samples_vs2017.sln
The relevant sourcecode can be found in samples/hellovr_opengl/hellovr_opengl_main.cpp

IMPORTANT: There is currently no detection in which way you are facing, so you might need to turn around for the calibration (change left and right feet) if right/left and up/down keys are wrong.
