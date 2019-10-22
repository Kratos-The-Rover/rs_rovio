# rs_rovio
## Rovio config files for Realsense RGB + IMU

### Steps:

* Build from source [rovio](https://github.com/ethz-asl/rovio)

* Copy the rovio_camr.yaml and rovio_custom.info file in cfg folder of rovio

1)roslaunch realsense2_camera rs_camera.launch enable_sync:=true unite_imu_method:=linear_interpolation

2)ROS_NAMESPACE=/camera/color rosrun image_proc image_proc

3)roslaunch rovio rovio_node.launch
