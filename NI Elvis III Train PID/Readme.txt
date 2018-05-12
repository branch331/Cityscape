Cityscape Project

Use camera feedback to control model train with PID.

SW Needed:
LV2018
LVRT2018
Vision Development Module 2018
Vision Acquisition 2018
myRIO2018 (for testing)
Elvis III 2018

To run program, do the following:
1. Power on the RIO; connect to PC with USB
2. Connect USB camera to PC
3. Connect C/AI0 to the remote controller's Fwd (gray, closer to the 'on' switch) and Gnd wires (orange/middle)
4. Open 'PID_Testing' project
5. Open the 'Object_TrackWebcam_PC.vi'
6. Open the 'PID_RT.vi'
7. Place camera above track
8. Run the webcam VI. Select a 'destination' point on the track, and then drag a square around the point of interest on the train.
9. Run the PID VI 

The train will move until it reaches the end point. It calculates the distance between the initial and end points and outputs
a proportional voltage.