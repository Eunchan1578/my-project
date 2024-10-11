# my-project
```mermaid
graph TD
    CM["CM (Command Center): PC<br>Human detection, gesture recognition"]
    IntelRealSense["Intel RealSense"]
    JetsonNano["Jetson Nano"]
    TurtleBot["Turtle Bot"]
    RemoteProtocol["Remote protocol: TCP/IP"]

    CM -->|Depth and color image| IntelRealSense
    CM -->|Turtlebot Command| TurtleBot
    JetsonNano -->|ROS2 control| TurtleBot
    TurtleBot --> RemoteProtocol
```

# HLD1
![HDL1](./HLD1.png)


# HLD2
![HDL2](./HLD2.png)



# HLD1
<img src="./HLD1.png" alt="이미지 설명" width="400" height="400"/>

# HLD2
<img src="./HLD2.png" alt="이미지 설명" width="300" height="300"/>




# finished job
1. ROS를 통한 turtle bot control Check
2. jetson nano와 intel realsense connection Check
3. 라즈베리에서 intel realsense 사용 불가 Check
4. mediapipe 를 사용한 hand gesture recognition Check


# current job
은찬, 태섭 : 통신 속도 정상화, turtlebot 제어 코드 refactoring, frame 처리 및 동작 제어 threading ,제스쳐 명령 수행
동현, 의근 : 
