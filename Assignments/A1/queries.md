In the 2nd part of the assignment, we are supposed to use: calibrateCamera() for camera Calibration as stated in the assignment.
But the function works only for planner objects, (i. e z=0). Refer to issue: https://github.com/opencv/opencv/issues/23586.
Can you please clarify the usage of this function for 3-D objects?

So, the calibrateCamera() function works on 3D objects when you are given an initial guess of an intrinsic matrix (see flags). Consider one of the walls as the z=0 plane and get an estimate. Then, refine the estimate based on world / image points from both walls. You can then discuss the differences between different estimates of the intrinsic / projection / rotation / translation components.
