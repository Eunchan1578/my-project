# my-project
```mermaid
graph TD
    subgraph CM[CM (command center): PC]
    A[Human detection, gesture recognition]
    end

    subgraph HW[Hardware]
    B[Intel Realsense]
    C[Jetson Nano]
    D[Turtle Bot]
    end

    CM -->|Depth & color image| B
    CM -->|Turtlebot Command| D
    HW -->|Control: ROS2 (dashing)| D
    E[Remote protocol: TCP/IP]
    D --> E
```
