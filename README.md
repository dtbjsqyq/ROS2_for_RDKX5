项目功能概述
1. 核心功能
机器人控制: 通过turn_on_wheeltec_robot包实现机器人的基础驱动控制
导航系统: 集成了完整的Navigation2系统，包括路径规划、避障、地图构建等功能
SLAM建图: 通过wheeltec_robot_slam和gmapping实现同步定位与地图构建
视觉处理: 包含相机驱动(usb_cam-ros2、astra_camera)和AR标记识别(aruco_ros)
2. 传感器支持
激光雷达: 通过wheeltec_lidar_ros2支持多种型号的激光雷达
摄像头: 支持USB摄像头和Astra深度摄像头
麦克风阵列: 通过wheeltec_mic支持语音识别和声音定位
3. 控制方式
键盘控制: 通过wheeltec_robot_keyboard实现键盘遥控
手柄控制: 通过wheeltec_joy支持游戏手柄遥控
自动路径跟踪: 通过wheeltec_path_follow实现路径自动跟随
4. 高级功能
自动充电: auto_recharge_ros2模块支持机器人自动寻找充电桩功能
目标跟踪: wheeltec_robot_kcf支持基于KCF算法的目标跟踪
跟随功能: simple_follower_ros2实现跟随特定目标的功能
RRT路径规划: wheeltec_robot_rrt2实现快速随机树路径规划算法
5. 可视化和监控
RViz2集成: 通过wheeltec_rviz2提供可视化界面
Web视频流: web_video_server-ros2支持通过Web浏览器查看机器人摄像头画面
6. 系统特点
基于ROS2 Humble版本开发
面向RDK X5机器人平台定制
模块化设计，便于功能扩展和维护
完整的机器人开发和竞赛解决方案
这个项目是一个功能齐全的ROS2机器人开发平台，集成了机器人控制、导航、感知、规划等核心功能，特别适合用于职业技能竞赛和机器人学习研究。

// src\turn_on_wheeltec_robot\launch\wheeltec_lidar.launch.py 中，记得改成自己雷达的型号