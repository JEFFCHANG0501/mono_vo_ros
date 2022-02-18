# mono_vo_ros
This is an OpenCV 3.0 based implementation of a monocular visual odometry algorithm.  
Note that this project is not yet capable of doing reliable relative scale estimation, 
so the scale informaion is extracted from the KITTI dataset ground truth files.  

## Before you run
In order to run this algorithm, you need to have either your own data, 
or else the sequences from [KITTI's Visual Odometry Dataset](http://www.cvlibs.net/datasets/kitti/eval_odometry.php).  
In order to run this algorithm on your own data, you must modify the intrinsic calibration parameters in the code.

install mono_vo_ros
```bash
$ mkdir -p ros_ws/src && cd ros_ws/src
$ git clone https://github.com/JEFFCHANG0501/mono_vo_ros.git

$ roslaunch mono_vo_ros mono_vo_ros.launch
```
