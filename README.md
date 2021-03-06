# Quadcopter Winter Project
## How to use

The quadcopter that was designed for this project is flown with an RC transmitter. The next step is to implement autonomous flight by connecting a Raspberry Pi 4 to the flight controller. Here's how to fly the drone using the RC:

1. Make sure that your batteries are fully charged. Secure the battery between the upper and lower frame using Velcro straps.
2. Attach the propellers to the motor shafts oriented correctly so that they provided an upward lift depending on the direction the motor spins. Fasten each propeller with the shaft nuts.
3. Connect the battery cable to the power distribution board cable.
4. Find a spacious area to fly, put on a pair of safety glasses, and step back from the drone about ten feet.
5. Turn on the transmitter, and arm the drone by bringing the throttle to zero and yaw to the right.
6. Keep the pitch and roll controls centered as you gently throttle up several feet off the ground.
7. Have fun flying!
8. When finished, slowly throttle down for a soft landing.

![Image of Quadrotor](images/drone.png)

## Materials
- F450 Quadcopter Frame Kit
- 4 Propellers (plus extras)
- 4 1000KV Brushless Motors
- 4 30A Electronic Speed Controllers
- CC3D Flight Controller
- 2.4GHz 6 Channel Digital Transmitter and Receiver
- 2700mAh 3s LiPo Battery
- XT60 Plug Male and Female Connector
- Battery Balance Charger / Discharger

## Block Diagram
![Image of Block Diagram](images/block_diagram.png)

## Receiver and Motor Diagram
![Image of Receiver and Motor Diagram](images/motor_receiver_diagram.png)

## Software
For this project, I used the open source program, LibrePilot, to calibrate the flight controller, ESCs, and trasmitter. LibrePilot can be downloaded [here](https://librepilot.atlassian.net/wiki/spaces/LPDOC/pages/4128780/Downloads).
I used [example code](examples/example.py) from the LibrePilot source code to attempt autonomous communication between a Raspberry Pi and the flight controller. However, writing over serial to the flight controller proved to be a challenge. 
