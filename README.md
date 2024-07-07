# Manipulate-with-turtlesim-package-in-ROS-noetic

After anstalling and setup ROS, now we are going to directly start a ROS node, and understand what is a ROS node

First, it is important to start a ROS master node using the command: 
```
roscore
```
![image](https://github.com/khawla-cs/Manipulate-with-turtlesim-package-in-ROS-noetic/assets/173630971/8762e500-7918-425a-9dce-d1f45650355e)

I am just going to try to start another ROS master in another terminal just to see what happens...

![Screenshot 2024-07-07 233420](https://github.com/khawla-cs/Manipulate-with-turtlesim-package-in-ROS-noetic/assets/173630971/3dbaff4b-9321-4fcd-a8c6-4de817b7bb47)

as you see we have an error here when we start a new ROS master. Why? because roscore can not run as another master is already running. so if you want to start a ROS master you can only have ONE.

## manipulate with some packages

#### 1-This command below it seems to be a program that is going to print "hello world" in the terminal with a timestamp
```
rosrun rospy_tutorials talker
```

![Screenshot 2024-07-07 234928](https://github.com/khawla-cs/Manipulate-with-turtlesim-package-in-ROS-noetic/assets/173630971/ca121e75-8888-4178-bda5-e63c714d0d3d)

if you want to stop the node you can press (ctrl + C)

#### 2- this is a ROS tool that allows you to have a graphical view of the actual ROS (nodes, topics and communications that are running on your computer)
```
rqt_graph
```
![Screenshot 2024-07-08 000901](https://github.com/khawla-cs/Manipulate-with-turtlesim-package-in-ROS-noetic/assets/173630971/36dc8b47-21e5-4e14-8e5a-947d8b64d8af)

you can see that here we have ONE node named (talker)

#### 3- this is another program that is going to print something in the terminal, and (heard) hello world with the timestamp. actually this data coming from the (talker) node
```
rosrun rospy_tutorials listener
```
![Screenshot 2024-07-08 002222](https://github.com/khawla-cs/Manipulate-with-turtlesim-package-in-ROS-noetic/assets/173630971/3ab7b796-d781-4e3c-8282-8015976e58e3)

## Turtlesim

1- This command is going to show a graphical window with a turtle
```
rosrun turtlesim turtlesim_node
```
![Screenshot 2024-07-08 003220](https://github.com/khawla-cs/Manipulate-with-turtlesim-package-in-ROS-noetic/assets/173630971/cc32539e-8b14-4dbf-90cd-8e9759916c60)

2- this command will allows you to control the turtle with aarrow keys of your keyboard

```
rosrun turtlesim turtle_teleop_key
```
![Screenshot 2024-07-08 004144](https://github.com/khawla-cs/Manipulate-with-turtlesim-package-in-ROS-noetic/assets/173630971/744a27f1-df51-4e01-9465-fdf3d58cf854)

note: if the turtle does not moving, make sure to click the terminal window that contains ( rosrun turtlesim turtle_teleop_key )command.






