# MobileRobot-Openloopcontrol
## Aim:

To develop a python control code to move the mobilerobot along the predefined path.

## Equipments Required:
1. RoboMaster EP core
2. Python 3.7

## Procedure
Step 1:
Initiate the MobileRobot.

Step 2:
Connect your PC with the MobileRobot.

Step 3:
Open Python program.

Step 4:
Program the movements of the robot using python code.

Step 5:
Execute the python program.

## Program
Python control code to move the mobilerobot along the predefined path.
Developed by: Aashima Nazreen Sayeed S
Register No.: 21500368
from robomaster import robot
import time

if _name_ == '_main_':
    ep_robot = robot.Robot()
    ep_robot.initialize(conn_type="ap")

    ep_chassis = ep_robot.chassis

    ep_chassis.move(x=2.7, y=0, z=0, xy_speed=0.75).wait_for_completed()

    ep_chassis.move(x=0, y=0, z=45, xy_speed=1).wait_for_completed()

    ep_chassis.move(x=3, y=0, z=0, xy_speed=0.75).wait_for_completed()
    ep_chassis.move(x=0, y=-0.2, z=0, xy_speed=0.75).wait_for_completed()
      
    ep_chassis.drive_speed(x=0.3,y=0,z=-17)
    time.sleep(15)

    ep_chassis.move(x=0, y=0.5, z=0, xy_speed=0.75).wait_for_completed()
 
    ep_chassis.move(x=2, y=0, z=0, xy_speed=0.75).wait_for_completed()

    ep_robot.close()


## MobileRobot Movement Image
![Screenshot (93)](https://user-images.githubusercontent.com/94828604/155051784-e80975d2-1913-4ce7-9da5-f9d3b80a290a.png)
start point:
![Screenshot (95)](https://user-images.githubusercontent.com/94828604/155052071-46658c62-423c-47e5-8e26-5a8f67ea308f.png)
End point:
![Screenshot (97)](https://user-images.githubusercontent.com/94828604/155052368-6ca7056a-2d74-410e-a57e-f6a0baa3f4d6.png)
Mobile robot movement image:
![Screenshot (99)](https://user-images.githubusercontent.com/94828604/155052624-0b1ab978-0866-4660-ad68-90353a476503.png)

## Result:
Thus the python program code is developed to move the mobilerobot in the predefined path.

Mobile Robotics Laboratory
Department of Artificial Intelligence and Data Science/ Machine Learning
Saveetha Engineering College

```
