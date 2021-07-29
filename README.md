# `ros_readbagfile`
Reads and prints all messages published on the specified topics from the specified ROS bag file

This is a modified version of the script [ros_readbagfile](https://raw.githubusercontent.com/ElectricRCAircraftGuy/eRCaGuy_dotfiles/master/useful_scripts/ros_readbagfile.py). I added some extra options, and here is its usage:

## Installation

Install dependencies:
    sudo apt install python-rosbag   # for python2 (deprecated)
    sudo apt install python3-rosbag  # for python3 (recommended)

Edit the shebang to `#!/usr/bin/python3` when using Python3

## Usage

Detail in: <https://www.codeinsideout.com/blog/ros/tutorial-beginner/#16-read-message-from-rosbag>

1. See the information of the input bag file:
```    
ros_readbagfile mybagfile.bag info
```

2. Print all messages of all topics in the bag file to the screen:
```
ros_readbagfile mybagfile.bag
```

3. Print all messages of the topic /test in the bag file to the screen:
```
ros_readbagfile mybagfile.bag /test
```

4. Print at most N first messages of all topics in the bag file to the screen:
```
ros_readbagfile mybagfile.bag N
```

5. Print at most N first messages of the topic /test in the bag file to the screen:
```
ros_readbagfile mybagfile.bag N /test
```

6. To save the output to a file, use redirection syntax:
```
ros_readbagfile mybagfile.bag N /test > output.txt
```

