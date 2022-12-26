# Closed_loop_System 
### This project mainly contains the closed loop system for the turtleism project.

###### This is a Publisher and Subscriber project in Python.

In the standard turtleism project we create a publisher in one node and a subscriber in another node, but in this there is a node with other nodes which contain both 
publisher as well as a subscriber that will help us to create closed loop system for the turtleism. 

![image](https://user-images.githubusercontent.com/112164785/209560951-68f903a8-e284-4275-a581-31c0239816d9.png)

From the above image we are trying to control the turtle in the tutleism node with the closed loop control.
For this we need to have the position(pose) of the turtle to know where the turtle is and we will need to send commands to the topic named 'cmd_vel'.

We are creating a node between the two that will subscribe to the '/turtle1/pose' node and publish it to the '/turtle1/cmd_vel' node.

The controller is used to control the turtle so that it can continously move around.
It also instructs it to move forward and to turn around and continue to move when it gets closer to the edge of the window.
