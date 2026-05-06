# ROS 2 Basics

A comprehensive collection of ROS 2 packages demonstrating core concepts including Communication Patterns (Pub/Sub, Services), Parameters, and Custom Interfaces using both **C++** and **Python**.

## Features

This repository is organized into specific packages to demonstrate the following ROS 2 pillars:

*   **C++ Packages:**
    *   `cpp_pubsub`: Basic Talker and Listener nodes.
    *   `cpp_service_client`: Service and Client implementation for request-response logic.
    *   `cpp_parameters`: Reading and updating node parameters at runtime.
*   **Python Packages:**
    *   `py_pubsub`: Minimal Publisher and Subscriber implementation in Python.
*   **Interfaces:**
    *   `tutorial_interfaces`: Custom `.msg` and `.srv` definitions (Internal Interfaces) used across the packages.

---

## Installation & Setup

### Prerequisites
*   **OS:** Ubuntu 22.04 (Jammy Jellyfish)
*   **ROS 2 Jazzy:** 
*   **Build Tool:** `colcon`

### Building the Workspace
1. **Create a workspace and clone the repository:**
   ```bash
   mkdir -p ~/ros2_ws/src
   cd ~/ros2_ws/src
   # Clone this repository (ensure the folder name matches your setup)
   git clone [https://github.com/arjjann/ros2_basics.git](https://github.com/arjjann/ros2_basics.git)

2. **Install dependencies using rosdep:**
   ```bash
   cd ~/ros2_ws
   rosdep install -i --from-path src --rosdistro humble -y

4. **Build the packages**
     ```bash
     colcon build
     source install/setup.bash

### Run the Packages
Before running any nodes , ensure you have sourced fines in every new terminal
  ```bash
      source ~/ros2_ws/install/setup.bash
```
Then runn packages as: ros2 run package node eg:- 
```bash
ros2 run cpp_pubsub talker
```

## Project Structure
In this project structure is as below:
ros2_basics/
├── cpp_parameters/ # C++ Parameter handling
├── cpp_pubsub/ # C++ Publisher/Subscriber
├── cpp_service_client/ # C++ Service/Client
├── py_pubsub/ # Python Publisher/Subscriber
└── tutorial_interfaces/ # Custom Msg/Srv definitions

## 📚 Resources & Documentation

For more information on the specific features and APIs used in this project, refer to the official documentation:

*   **[ROS 2 Jazzy Documentation](https://docs.ros.org/en/jazzy/index.html)** - Official guide for Jazzy Jalisco.
*   **[ROS 2 Jazzy Tutorials](https://docs.ros.org/en/jazzy/Tutorials.html)** - Official beginner and advanced tutorials.
*   **[ROS 2 Jazzy Release Notes](https://docs.ros.org/en/jazzy/Releases/Release-Jazzy-Jalisco.html)** - Details on new features and changes in this version.

---


## License
Distributed under the Apache License 2.0. See `LICENSE` for more information.

---

**Author:** [Arjan](https://github.com/arjjann)






