# Turtlesim
The terminal that I am using is in ROS_DISTRO=foxy and can also be checked by the given command below.

```
printenv | grep -i ROS
```
(![image](https://github.com/sanjiblama28/Github/blob/main/11.PNG)

## 1. Turtlesim: Installation
First of all,  making sure your system is up-to-date and then installing the turtlesim library along with checking that the package is installed by the following command.

```
sudo apt update
sudo apt install ros-foxy-turtlesim
ros2 pkg executables turtlesim
```
![image](https://github.com/sanjiblama28/Github/blob/main/12.PNG)

## 2. Turtlesim: Start

Enter the following command to start turtlesim in your terminal:
```
ros2 run turtlesim turtlesim_node
```
Now, the simulator window appears along with a turtle in the center and messages from the node can be seen in the terminal.    

![image](https://github.com/sanjiblama28/Github/blob/main/13.PNG)
## 3. Use Turtlesim
Now, the new terminal needs to be opened and the following command needs to be executed to control the turtle type.
```
ros2 run turtlesim turtle_teleop_key
```
![image](https://github.com/sanjiblama28/Github/blob/main/l.PNG)

You should have three windows open at this point:
```
a terminal running turtlesim_node 
a terminal running turtle_teleop_key 
the turtlesim window
```

# RQT
## 4. Installation of RQT
Now, You need to open a new terminal to make sure your system is up-to-date and then install the rqt library and its plugins and to use rqt by the given command below.

```
sudo apt update
sudo apt install ~nros-foxy-rqt*
rqt
```
![image](https://github.com/sanjiblama28/Github/blob/main/141.PNG)

![image](https://github.com/sanjiblama28/Github/blob/main/14.PNG)


## 5. RQT: Running 
The window will be blank for the first time use of rqt. Then you need to select Plugins > Services > Service from the menu bar at the top.
![image](https://github.com/sanjiblama28/Github/blob/main/15.PNG)

## 5.1 Trying some of the services provided by service caller

Select the /spawn service where the /clear is seen and can also be used to select other services also and /spawn will help in creating another turtle in the turtlesim window by replacing the digit 0 with another digit and string name also needs to be written and the result can be seen in the response and the turtlesim window.

![image](https://github.com/sanjiblama28/Github/blob/main/161.PNG)

![image](https://github.com/sanjiblama28/Github/blob/main/162.PNG)

Now, using teleport_abosulte service as shown in the figure below.

![image](https://github.com/sanjiblama28/Github/blob/main/s1.PNG)

![image](https://github.com/sanjiblama28/Github/blob/main/s2.PNG)


## 6. RQT: rqt_console

A GUI tool called rqt_console is used in ROS 2 to inspect log messages.
With the following command, you can start rqt_console in a new terminal:
```
ros2 run rqt_console rqt_console
```
![image](https://github.com/sanjiblama28/Github/blob/main/17.PNG)

The console's first part is where the system log messages from your system will appear.
In the center, you can exclude severity levels to filter out messages.
The mails with your custom string are highlighted in the bottom portion.

