# Flying robot

![Quad Image](images//IMGP1502.JPG)

[A flying robot has been built as a development platform.](https://github.com/PhilippeDoucette/Intel-RTF-Drone-with-servo-control/wiki)  Servers are networked with the robot to provide related processing. Multiple robots may participate in this Client/Server architecture, used to reduce the computational load on the robots.  Most processing is done on servers, while robots act as clients.  The robots may then have smaller computers and lower cost. The servers share workload among many robot-clients. Computation that would be difficult or impossible to perform on the robot is done on the servers.  

| Server-side              | Client-side               |
| ------------------------ |---------------------------|
| Large dataset queries    | Stablility and movement   |
| Human voice processing   | Speech and sound output   |
| Image recognition        | Sensor polling            |
| Swarm coordination       | Servo control             |
| Long-range path Planning | Short-range path planning |

The robot consists of several computer types, each appropriate for its task. An [Intel Aero Compute Board](https://software.intel.com/en-us/aero/compute-board) runs Ubuntu , which hosts [ROS](http://www.ros.org), GPS, IMU, and other flight related tasks.  An [Arduino Due](https://store.arduino.cc/usa/due) is used to interfaces sensors, servos, and LED's.  An [Intel RealSense](https://www.intel.com/content/www/us/en/architecture-and-technology/realsense-overview.html) is used for on-board image processing.

## Example Application
Searching for a lost person would require image processing, long-range navigation, voice processing, and other computationally intensive tasks that are best run on a server.  The robot would be connected to the internet via Wi-Fi or a cellular data network.  Servers would be datacenter located. High-level human control would be done via workstation or mobile device. Public internet connects everything.


![Search and Rescue](images/Search_and_Rescue.jpg)

## Hardware

Intel® RTF Drone connected to an Arduino provides a powerful ROS computer with simple connections to external devices. All manner of servos, stepper motors, and a vast array of sensors may be connected to a flying/driving robot platform. The Intel system runs ROS Ubuntu and connects to the Arduino using RosSerial.

## Systems
### Intel RTF Drone
* Intel Atom 64 bit computer running Ubuntu & ROS
* Global positioning system (GPS)
* Inertial measurement unit (IMU) 
* Wi-Fi as access point or connectivity to LAN
* Celluar modem connectivity to internet
* Flight controller
* Electronic Speed controllers (ESP) for rotors
* RealSense 3D camera
* Forward camera
* Dowward camera
* MicroSD card slot
* Beacon LED's
* 18 channel Micro Serial Receiver DSMX 2.4GHz RF (Radio Control)
* HDMI monior output
* USB 3 connetion for mouse and keyboard
### Arduino Due
* [Differential drive wheels](https://github.com/PhilippeDoucette/Flying-Robot/wiki/Differential-drive-wheels)
* Servo controllers
* Stereo amplifier and speakers
* Text-to-speech speech system and speaker
* MicroSD card slot
* White bright LED's for area illumination
* Tri-color bright LED's as emergency display lights


(wiki/Differential-drive-wheels)


This site is under development, documenting the current state of the project
