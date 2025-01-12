# IMU-study

本项目是“瞰百易”计划的一部分

![0](README.assets/0.jpg)

对常见IMU芯片的原理、驱动和数据融合算法整理，以区分某度、某坛上面碎片化严重到影响入坑的乱象。

注：角加速度、角速度的融合算法中，卡尔曼滤波（参考网上）、类一阶滤波（一阶滤波算法改的）和清华滤波（本科智能车竞赛常用的）这三种算法的具体 C 语言实现的代码，已经写在了我的另一个项目 MCU Framework 的 IMU Device 中，[链接](https://github.com/Staok/stm32_framework/tree/master/STM32F4DSP_HAL_freeRTOS_Framework/DEVICES/IMU)。

目录树形图：

```
├─0 加速度计、陀螺仪介绍
├─1 IMU的惯导、数据融合文档
│  ├─卡尔曼介绍
│  ├─四元数-欧拉角
│  └─数据融合、姿态解算
│      └─一种数据融合，算量有点大，没看懂
├─2 MPU系列传感器资料
│  ├─MPU-6050中文资料、测试程序和硬件资料
│  │  ├─MPU-6050官网资料
│  │  ├─原理图
│  │  ├─寄存器描述 使用心得
│  │  └─测试程序
│  ├─MPU-6500官网资料
│  ├─MPU-9250官网资料、测试程序和硬件资料
│  │  ├─原理图
│  │  └─测试代码
│  ├─MPU-9255官网资料、测试程序和硬件资料
│  │  └─微雪百科方案
│  └─MPU_DMP官网库和说明
│      ├─motion_driver-5.1.3
│      └─motion_driver_6.12
├─3 其他各种IMU
│  ├─ADXL345 三轴加速度计
│  ├─ENC03 模拟 单轴陀螺仪
│  ├─HMC5883L 电子罗盘
│  │  ├─原理图
│  │  └─官方手册 使用经验
│  │      └─官方手册
│  ├─ICM20602 六轴
│  ├─ICM20948 性能远超MPU6050 9250等，功耗更低
│  │  ├─ICM20948 官网资料全
│  │  │  ├─Chip
│  │  │  │  ├─App Notes
│  │  │  │  ├─Datasheet
│  │  │  │  └─User Guides
│  │  │  └─demo板
│  │  │      ├─Hardware Reference Design
│  │  │      ├─Product Brief
│  │  │      ├─Software
│  │  │      └─userguide
│  │  └─微雪百科方案
│  ├─IST8310 电子罗盘
│  ├─L3G4200 三轴陀螺仪
│  ├─MMA7455 三轴加速度计
│  ├─MMA8451 三轴加速度计
│  └─TDK-InvenSense Motion Sensor
├─README.assets
└─传感器的校准
```

