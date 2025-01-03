Note: The project files are stored in another repositary, because it is too large.
This README file is placed here for reference only.

***********************************************************************************************************
Start the simulator by running each command in its own terminal.
***********************************************************************************************************

1) Open Manipulator Robot Simulator
roscore
roslaunch open_manipulator_gazebo open_manipulator_gazebo.launch
roslaunch open_manipulator_controller open_manipulator_controller.launch use_platform:=false

In order to control the simulated OpenMANipulator-x,
	1a) start the OpenMANipulator control GUI
	roslaunch open_manipulator_control_gui open_manipulator_control_gui.launch

	OR  
	1b) keyboard remote operation
	roslaunch open_manipulator_teleop open_manipulator_teleop_keyboard.launch


2) Braccio Robot Simulator
roslaunch braccio_moveit_gazebo rviz_connected_with_gz_using_moveit.launch
rosrun braccio_moveit_gazebo target_object_sim.py

3) Intel RealSense D415
roslaunch realsense2_description view_d415_model_rviz_gazebo.launch

4) Webcam
roslaunch realsense2_description webcam_camera.launch

