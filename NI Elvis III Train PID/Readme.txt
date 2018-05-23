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
4. Set RT PID VI as a startup application on the Elvis target if not already
5. Have RT PID VI running
7. Place camera above track
8. Run the host application (NI Elvis III Train PID.exe)
8. Run the webcam VI. Select a 'destination' point on the track => enter
9. Drag a square around the point of interest on the train.
10. Click run -> click point on track on new popup -> enter

The train will move until it reaches the end point. It calculates the distance between the initial and end points and outputs
a proportional voltage.

**Notes from NIWeek 2018 for improvement:
-disable stop button when running so it can't be stopped mid-run
-encoding vi sometimes does not show
*make UI more intuitive/faster. clicking the run button and waiting for image to click on takes way to long to show up