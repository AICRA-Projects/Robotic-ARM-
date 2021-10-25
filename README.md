# Robotic-ARM
## The Industrial Robotic Arm
An industrial robot arm is a marvel of engineering in that it reacts similarly to our own arms. The robot arm closely resembles a human arm, with a wrist, forearm, elbow and shoulder. The six-axis robot has six degrees of freedom, allowing it to move six different ways, unlike the human arm, which has seven degrees of freedom.
Industrial robotic arms move much faster than human arms and, without the proper safety measures, can be dangerous. Robotic arms usually have some form of safety package or sensors available to ensure the safety of human workers.
An industrial robot arm not only increases the speed of the manufacturing process, but also the accuracy and precision. These robotic arms cut down on worker error and labor costs.The industrial robotic arm, which is usually made of steel or cast iron is built from the base up, ending with the wrist and whatever end effector is needed to perform the arm’s chosen task. A robotic controller rotates motors that are attached to each joint. Some of the larger arms, used to lift heavy payloads, are run by hydraulic and pneumatic means.
The arm’s job moves the end effector from place to place – picking up, putting down, taking off or welding a part or the entire work piece. These robotic arms can be programmed to do several different jobs or one specific job, depending on the manufacturer’s specifications and needs.
# Robotic arm configuration 
The Robotic Arm has a 180° rotation angle and can provides 6 degrees of freedom. This included a parallel jaw gripper with a maximum opening span of 55mm.
High Torque Standard Servo Motor with Metal Gears. Provides 11kg/cm at 4.8V, 13.5kgcm at 6V and 16kg/cm at 7.2V.

## How to operate:
### step 1: It has two state pick and place with light indication Red Led and Green Led 
### step 2: Green LED "ON" place the object and Gripper mouth is Open 
### step 3: Red Led "ON" means pick and gripper mouth will get close
## Circuit Diagram
![Robotic ARM (1)](https://user-images.githubusercontent.com/42414598/137720141-85d5d5e9-83cd-4863-8c67-ab38e0b8ad97.png)

## robotic arm gripper
![metal-gripper-for-robot-arm-sunrobotics-original-imag4gxkzvjkgmjc](https://user-images.githubusercontent.com/42414598/138668684-c8544cc6-ceaf-41b4-b0f9-ef32a2721647.jpeg)


## Features:
* Rotation angle of 180 degrees
* Height: 46cm
* Clamp Max opening: 55mm
* Color: Black chassis 
* Metal Gripper 
* 360 Modifiable: Yes
* Potentiometer Drive: Indirect Drive
* Bearing Type: Double Ball Bearing
* Gear Type: All Metal Gears
* Connector Wire Length: 12"
* Dimensions: 1.6" x 0.8"x 1.4" (41 x 20 x 36mm)
* Weight: 56gm
## Robotic arm Components:
* 6 x Metal Gear Standard Servo Economy
* 4 x Multipurpose Aluminium Standard Servo Bracket
* 1 x Long U Aluminium Servo Bracket
* 2 x Short U Shape Aluminium Servo Bracket
* 2 x L Shaped Interconnect Servo Bracket
* 1 x Parallel Jaw Robotic Gripper
* 6 x Metal Horn for Servo 25T
* 3 x Bearings
* 1 x Rotating base assembly
* 1 x Screw nut set
## Servo Motor Features:
* The unit comes complete with 30cm wire and 3 pin 'S' type female header connector that fits 
most receivers, including Futaba, JR, GWS, Cirrus, Blue Bird, Blue Arrow, Corona, Berg, 
Spektrum and Hitec. 
This high-speed standard servo can rotate approximately 120 degrees (60 in each direction). 
You can use any servo code, hardware or library to control these servos, so it's great for 
beginners who want to make stuff move without building a motor controller with feedback & 
gear box, especially since it will fit in small places. The MG995 Metal Gear Servo also 
comes with a selection of arms and hardware to get you set up nice and fast!
## Servo Specification:
* Weight: 55 g 
* • Dimension: 40.7 x 19.7 x 42.9 mm approx. 
* • Stall torque: 8.5 kgf·cm (4.8 V ), 10 kgf·cm (6 V) 
* • Operating speed: 0.2 s/60º (4.8 V), 0.16 s/60º (6 V) 
* • Operating voltage: 4.8 V a 7.2 V 
* • Dead band width: 5 µs 
* • Stable and shock proof double ball bearing design 
* • Temperature range: 0 ºC – 55 ºC
## Microcontroller Board:
Arduino is an open-source platform used for building electronics projects. Arduino consists of both a physical programmable circuit board (often referred to as a microcontroller) and a piece of software, or IDE (Integrated Development Environment) that runs on your computer, used to write and upload computer code to the physical board.

The Arduino platform has become quite popular with people just starting out with electronics, and for good reason. Unlike most previous programmable circuit boards, the Arduino does not need a separate piece of hardware (called a programmer) in order to load new code onto the board -- you can simply use a USB cable. Additionally, the Arduino IDE uses a simplified version of C++, making it easier to learn to program. Finally, Arduino provides a standard form factor that breaks out the functions of the micro-controller into a more accessible package.
* Arduino UNO R3 x 1
## Control and Methodology: 
* This project is based on Introduction to "how does robotic arm works?", This is designed with detachable components which can be setup accorading to the needs which provides the user to calculate and produce required Ouptut
* Here we have used three arduino boards to control multiple joints and gripper in the robotic arm 
* Each one connected with 2 or 3 sets of servo motor and provides a good stablity during the movement of links 
* Here we have defined the working of the robotic arm with code which are lower_joints_links, upper_joints_links and gripper 
#### Lower_joints_links
Here its defined for controlling the lower joints as per the measurement first and second lower joints consume more potential difference then upper joints , we have seperated the code and arduino due to excess consumption of power , we have decrease the Normal force or torque due to normal force by fixing the angle where joints can over come from high torque 
Code is defined with different position value or angle value of three servo motors which can be manipulate or change by the user
* base servo_motor_j 0 < angle < 180
* middle servo_motor_t 30 < angle < 120 (bears the maximum torque)
* upper middle serve_motor_k 0 < angle < 90
#### Upper_joints_links  
Here its defined for controlling the upper joints, we have seperated the code and arduino due to excess consumption of power , we have decrease the Normal force or torque due to normal force by fixing the angle where joints can over come from high torque 
Code is defined with different position value or angle value of three servo motors which can be manipulate or change by the user
* upper joint servo_motor_j 0 < angle < 180
* gripper_joint servo_motor_k 0 < angle < 180 
#### Gripper 
This script is the simplest one which has two output state defined by two leds and one servo motor to direct the state of gripper of servo motor , Here we have defined the condition of led on and off by dependinf on ther servo motor angle which is corresponding to the gripper open and close state
Code is defined with different position value or angle value of three servo motors which can be manipulate or change by the user
* gripper servo_motor 0 < angle < 180
* RED LED on Gripper is closed 
* Green LED on Gripper is open 
## Conclusion:
Robotic arm has use in various industries from manufacturing Cars to packaging, from using versatile task to being used in for repetitive jobs. Robotics have a special use in manufacturing as it gives a wide range to tool that can be connected with it and hence again versatility in useage.
## Refernce:
* https://components101.com/motors/mg995-servo-motor
* https://robokits.co.in/robot-kits



