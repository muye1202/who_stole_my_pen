# Who stole my pen?
The pincher-X 100 robot arm plucks a pen from the user's hand.

This project contains implementation of a image pipeline that can recognize the pen (or other object) in the range of the camera and outputs the centroid of the object, which is then sent to the robot arm control unit that guides the end-effector to this position and grasps the pen.

## Demo


https://user-images.githubusercontent.com/112987403/210007021-ae27e4e0-4ece-44a0-bd2a-e76abe74a57c.mp4


## Note
The image processing unit can be tuned to return the centroid of any object: run the image_pipeline.py with
RealSense camera connected, and use the slide bars to tune the color mask until only the desired object
is visible in the image; replace the a b c d values with the slide bar values; and the algorithm should be able
to return the centroid of the object, which can then be used as the grasping point of the robot arm.


## Acknowledgement
Thanks for the image alignment example provided by librealsense made by Intel.

Their git repo: https://github.com/IntelRealSense/librealsense/blob/master/wrappers/python/examples/align-depth2color.py
