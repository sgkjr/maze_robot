# maze_robot
Program to control a LEGO rebot within a maze and trace the shortest path to the intial point from the  destination.
 During the forward motion a 2D array is filled with incrmental weights starting from 1 whenever
robot  takes that particular path. To find the shortest return path, three adjacent array elements are 
compared and the positon with least weight is chosen as the next direction of travel. This is continued till 
the intial starting position is reached

Motor ports
------------
Motor A - Wheel right
Motor C - Wheel left
Motor B - light sensor rotation

Sensors
-------
Port 4 - Light Sensor
port 3 - Ultrasonic Sensor


A sample map trace represented in 2D array.
Robot started from the 'start' and added weights to each 
location it traced. eight of 2 reresent that position 
was traced twice. '30' represents a dead end.

0 0 0 0 0 0 0 0 0
0 ______________
0 | 1   1_1_1_1_end|
0 | 1 | 0  0 0 0 0
0 | 1 |__________ 
0 | 2  _2_2_2_2_30|
0 | 1 | 0 0 0 0 0
0 | 1 | 0 0 0 0 0
  start
