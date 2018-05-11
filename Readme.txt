This program utilizes the onboard RTOS of the NI Elvis III to perform PID control on a model train.

The RT program is set as startup on the Elvis III and reads position data from the host program
taken from a camera using NI Vision software. The RT program then uses PID functions to control
the model train. 

The VIs also decode analog waveform data sent from another NI Elvis III.

To run:
-Connect to Elvis III
-Set RT Train PID as startup (or just run it)
-Calibrate camera using 'Calibrate_Camera' VI and NI MAX
-Run Host Train PID program
-Select center point -> enter
-Select ROI on train -> enter

Repeat:

-Click Run
-select destination on track -> enter