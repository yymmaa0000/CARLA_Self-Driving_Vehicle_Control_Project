# CARLA_Self-Driving_Vehicle_Control_Project
This project aims to develop a vehicle controller to control the vehicle in CARLA simulator to follow a race track by navigating through preset waypoints. The vehicle needs to reach these waypoints at certain desired speeds, so both longitudinal and lateral control were implemented on the vehicle.

This project is a part of the Self-Driving Cars Specialization course in Coursera. The detail about this specialization can be found [here](https://www.coursera.org/specializations/self-driving-cars).

The performance of the controller was simulated using the CARLA simulator, which is a modified version of the original CARLA simulator with additional maps included. If you wish to try my controller yourself, please download and install this simulator following the instructions [here](https://www.coursera.org/learn/intro-self-driving-cars/supplement/pGdcu/carla-installation-guide). To learn how to use this simulator, you can refer to the project instruction from Coursera website [here](https://www.coursera.org/learn/intro-self-driving-cars/programming/ac8R5/final-project-self-driving-vehicle-control).

In this project, I implemented 3 different controllers, which are:
1. PID for longitudinal and pure pursuit for lateral
2. PID + feedforward for longitudinal and pure pursuit for lateral
3. PID + feedforward for longitudinal and Stanley controller for lateral

These three controllers were stored in the “Working Controllers” folder. By replacing the controller2d.py file in the main directory, you can simulate different controllers CARLA. The simulation result for each controller is also stored in that folder.

The screen recording of the simulation for 2 controllers can also be viewed in YouTube:

PID + feedforward for longitudinal and pure pursuit for lateral: https://youtu.be/u6LND5ZGQ9c

PID + feedforward for longitudinal and Stanley controller for lateral: https://youtu.be/uTBMOVf5YPY

### Speed profile comparison between PID and PID+feedforward controller: ###

From the following two plots, it can be seen that the feedforward controller helps to eliminate the lag between the reference and actual speed.

#### PID controller: ####

![alt text](https://github.com/yymmaa0000/CARLA_Self-Driving_Vehicle_Control_Project/blob/master/Working%20Controllers/PID%20and%20Pure%20Pursuit/controller_output/Speed%20Profiles.png)

#### PID + feedforward controller: ####

![alt text](https://github.com/yymmaa0000/CARLA_Self-Driving_Vehicle_Control_Project/blob/master/Working%20Controllers/PID%20%2B%20feedforward%20and%20Pure%20Pursuit/controller_output/Speed%20Profiles.png)
