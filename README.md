# crazyflie-CAD

This directory contains SolidWorks files related to our quadrotor research in the MIT CSAIL Robot Locomotion Group (http://groups.csail.mit.edu/locomotion/) with the CrazyFlie platform.  More information about the CrazyFlie platform may be found at http://www.bitcraze.se/

There are two primary goals for the files in these directories:

-1 To find estimates for physical parameters (including inertia matrices) of the CrazyFlie hardware

-2 To design an ultra-lightweight frame that aids with motion-capture-based (i.e., VICON) control

The most recent iterations of the complete Solidworks models may be found in:

- Crazyflie-1-AssemblywithFrame/ (for the Crazyflie 1.0)
- Crazyflie-2-AssemblywithFrame/ (for the Crazyflie 2.0)

For goal (1) above, in order to get an approximate estimate of physical parameters that are important for model-based control (most notably, the inertia matrix I), an approximate model with accurate densities of individual components was built.  Refer to the assembly files.

For goal (2), the majority of these files are iterations of designing an ultra-lightweight frame that adds the scaffolding for motion-capture (VICON) markers to be attached. The markers placed on these frames create a motion-capture object with sufficient distance between markers and uniqueness of relative orientations.  With such a small (90 mm diagonal wheelbase) frame, it is difficult for a motion-capture system to identify the orientation of the object without the additional "wingspan" between markers added by the frame.  (Motion-capture systems may be more precise if the cameras are closer, but then the range of motion of the quadrotor is limited.)



## CrazyFlie-1

Directories that start with CrazyFlie-1 contain files for the CrazyFlie 1.0:

- Crazyflie-1-frames-prototypes/ contains prototypes of different frames 
