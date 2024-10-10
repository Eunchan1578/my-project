# my-project
```mermaid
graph TD
    CM["CM (Command Center): PC\nHuman detection, gesture recognition"]
    IntelRealSense["Intel RealSense"]
    JetsonNano["Jetson Nano"]
    TurtleBot["Turtle Bot"]
    RemoteProtocol["Remote protocol: TCP/IP"]

    CM -->|Depth & color image| IntelRealSense
    CM -->|Turtlebot Command| TurtleBot
    JetsonNano -->|Control: ROS2 (dashing)| TurtleBot
    TurtleBot --> RemoteProtocol
```
