## IIWA STACK Kitting Cell
[![Build Status](https://travis-ci.org/IFL-CAMP/iiwa_stack.svg?branch=master)](https://travis-ci.org/IFL-CAMP/iiwa_stack)

This is the ROS Indigo/Kinetic metapackage for the KUKA LBR IIWA R800/R820 (7/14 Kg). This was originally forked from [iiwa_stack](https://github.com/IFL-CAMP/iiwa_stack).

This package has been modified to be used with the [KUKA_IIWA_KITTING_CELL Project](https://github.com/bharatm11/Kuka_IIWA_Kitting_Cell_Final)

This package provides additional functionalities which can be used for the simulation of KUKA IIWA manipulators on Gazebo and Moveit. These functionalities include:
1) Simulation of a vacuum gripper - Branch: master
2) Simulation of a RGB camera at the end effector - Branch: camera_ee

**This package is meant to be used with version : v-1.2.0 for Sunrise 1.10 - 1.14**   
For use with a a previous version of Sunrise, please check out the documentation at:  (https://github.com/SalvoVirga/iiwa_stack/wiki/FAQ#which-version-of-sunriseossunrise-workbench-is-supported)    



### Features
- Native ROSJava nodes running on the robot as a Sunrise RoboticApplication: supports ROS parameters, topics, services, etc.
- Integration of KUKA's SmartServo motions:
  - joint position, joint velocity and cartesian position control via simple ROS messages. 
  - online configuration of JointImpedance, CartesianImpedance, DesiredForce and Sine(Force)Pattern via ROS service.
  - online configuration of joint velocity and acceleration via ROS service.
  - updates on the time left to reach the commanded destination via ROS service.
- The Sunrise tool to use can be selected via a ROS parameter.
- Gravity compensation by setting the appropriate JointImpedance values.
- NTP synchronization with a server running on the ROS master
- full MoveIt! integration
- Gazebo support
- Simulation of a vacuum gripper in Gazebo
- Simulation of a RGB camera at the end effector

___
### Usage
__The features and usage of the stack are described in depth on its  [WIKI][8].__  
We **_strongly_** suggest to have a look at the wiki to have a better understanding of the code, both for its use and its extension.     
Do you have problems? First, please check the [**FAQs**](https://github.com/SalvoVirga/iiwa_stack/wiki/FAQ). Issues or emails are always welcome!

**This package is meant to be used with version : v-1.2.0 for Sunrise 1.10 - 1.14**   
For use with a a previous version of Sunrise, please check out the documentation at:  (https://github.com/SalvoVirga/iiwa_stack/wiki/FAQ#which-version-of-sunriseossunrise-workbench-is-supported)    

___

### References
1. Hennersperger, Christoph, Fuerst, Bernhard, Virga, Salvatore, Zettinig, Oliver, Frisch, Benjamin, Neff, Thomas & Navab, ..*Nassir (2017). Towards MRI-based autonomous robotic US acquisitions: a first feasibility study. *IEEE transactions on ..*medical imaging*, 36, 538-548.

### Acknowledgements
This repository takes inspiration from the work of :
- _Centro E. Piaggio_ and their [ROS interface for the KUKA LBR 4+][1]
- _Mohammad Khansari_ and his [IIWA-ROS communication inteface][2] 
- _Robert Krug_ and his [IIWA URDF and Gazebo package][7]      
- _Li Huang_ and his [ur5_ROS-Gazebo package][9]
- _Salvatore Virga_ and his [iiwa_stack package][10]


[1]: https://github.com/CentroEPiaggio/kuka-lwr
[2]: https://bitbucket.org/khansari/iiwa.git
[3]: https://bitbucket.org/khansari/iiwa/src/c4578460d79d5d24f58bf94bd97fb6cb0b6f280f/msg/IIWAMsg.msg
[4]: https://bitbucket.org/khansari/iiwa/wiki/Home
[5]: https://bitbucket.org/khansari/iiwa/src/c4578460d79d5d24f58bf94bd97fb6cb0b6f280f/JavaNode/?at=master
[6]: http://git.lcsr.jhu.edu/cgrauma1/kuka_iiwa_shared
[7]: https://github.com/rtkg/lbr_iiwa
[8]: https://github.com/SalvoVirga/iiwa_stack/wiki
[9]: https://github.com/lihuang3/ur5_ROS-Gazebo
[10]: https://github.com/IFL-CAMP/iiwa_stack
