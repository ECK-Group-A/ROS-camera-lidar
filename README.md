# Install ROS

To view the data from the camera and the LIDAR, a program called ROS (Robotic Operating Systems) is required. This is a Linux based program which can collect and show data from the LIDAR and the camera. For this project, the ROS-version noetic is used, but it should be possible to use other versions as well. To install ROS, use the following commands:


`$ sudo sh -c 'echo "deb http://packages.ros.org/ros/ubuntu $(lsb_release -sc) main" > /etc/apt/sources.list.d/ros-latest.list'`

install curl if not installed yet <br />
`$ sudo apt install curl`

`$ curl -s https://raw.githubusercontent.com/ros/rosdistro/master/ros.asc | sudo apt-key add -`

`$ sudo apt update`

`$ sudo apt install ros-noetic-desktop-full`

when the installation is succesful, ROS can be used. A useful thing to add to the bash, is the following command:

`$ echo "source /opt/ros/noetic/setup.bash" >> ~/.bashrc`

After doing this command, it is not required anymore when opening a new terminal to add every time the source command for ROS.

To make use of ROS type: `$ roscore` and open up a new terminal.

Another useful feature to install is the command some python functions and rosdep. This can be done as followed:

`$ sudo apt install python3-rosdep python3-rosinstall python3-rosinstall-generator python3-wstool build-essential'

`$ sudo rosdep init`

`$ sudo rosdep update`

# Lidar

