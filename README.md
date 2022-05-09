# Research Track 2: Jupyter Notebook
## Description of the assignment
Starting from the third assignment of the course of Research Track 1 we have to create a jupyter notebook to interact with the simulation of it, that will be able to:
1. Switch to the different modalities, and manage them
2. Plot the robot position, the laser scanner data and reached / not reached targets

## How to install and run the code
To use the jupyter user interface, first is necessary to launch the ROS environment with these three launcher: 
```
roslaunch final_assignment simulation_gmapping.launch
```
```
roslaunch final_assignment move_base.launch
```
```
roslaunch RT2_jpy_assignment jpy_launch.launch
```
 And then open the jupyter notebook:
```
NB_assignment_3.ipynb
```
 

## Structure of the code
The graphic interface allows the user to choose if he wants the robot to reach a point, or if he prefers to guide the robot himself.  
In the first case, the interface will allow the user to enter the coordinates (x, y) of the target, and start the task by pressing the "start" button or cancelling the operation using the "undo" button.  
In the second case, 9 different buttons are displayed that can be used to guide the robot, and in addition the map on which it moves is displayed.
There is also a slider to allow the user to choose if he wants help in guiding the robot, blocking it before it collides with walls.  
Also in this case is present the "undo" button.  
In any case, three graphs are continuously displayed and updated. The first shows the path taken by the robot. The second shows the data from the laser scanner. While the third shows a histogram of the targets reached or not by the robot.


## Some issue
Although apparently convenient a single interface that allows you to control the robot, unfortunately the interface is very slow.  
The most significant example is the slowdown suffered by the robot when it is assigned a task to achieve, which also puts the graphs on hold.
Also, even when the user chooses to drive the robot, the button "responsiveness" is low and the graphics update is very slow.

## 
**Authors:** Daria Berretta

