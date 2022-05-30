To view the data from the camera and the LIDAR, a program called ROS (Robotic Operating Systems) is required. This is a Linux based program which can collect and show data from the LIDAR and the camera. For this project, the ROS-version noetic is used, but it should be possible to use other versions as well. To install ROS, use the following commands:


`$ sudo sh -c 'echo "deb http://packages.ros.org/ros/ubuntu $(lsb_release -sc) main" > /etc/apt/sources.list.d/ros-latest.list'`

install curl if not installed yet
$ sudo apt install curl

$ curl -s https://raw.githubusercontent.com/ros/rosdistro/master/ros.asc | sudo apt-key add -

$ sudo apt update

$ sudo apt install ros-noetic-desktop-full


