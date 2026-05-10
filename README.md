
<p align="center">
  <a href="#chinese-version"><b>简体中文版本</b></a> | <a href="#english-version"><b> English Version</b></a>
</p>

---

<a name="chinese-version"></a>
##  简体中文版本

### 个人简介

你好！我是 **麦克斯**。本科机器人学在读生。

目前研究方向为**具身人工智能（Embodied AI）**，具体包括**足式机器人的强化学习 (RL) Locomotion** 算法及其物理实体部署。

工程实践中，将运动学闭链解算、LQR/VMC 等数学方法与 AI 算法结合，应用于双足平台与高机动底盘的运动控制。


### 核心项目精选（目前各项目仍在整理中，每个项目本地完成整体梳理后会完整推送到github中，目前在集中处理BPIC项目）

* **[RooCode Plus — 多模型本地代理适配层](https://github.com/Tensor-0/roocode-plus)**
  针对 Roo Code 的多模型本地代理适配层。基于 FastAPI 构建本地服务拦截与重构 HTTP 请求，动态注入缺失参数，解决 Roo Code 与 DeepSeek 等模型间的 API 格式不兼容及上下文截断问题。包含跨平台自动化安装与测试脚本。
  `Python` `FastAPI` `Shell`

* **[DBRL: 达妙双足机器人强化学习框架](https://github.com/Tensor-0/dbrl-damiao-bipedal-rl)**
  针对达妙 19 自由度双足机器人的 RL 步态优化框架，包含 Isaac Gym 仿真环境搭建、策略训练，以及 ONNX 模型在物理硬件上的 Sim-to-Real 部署。
  `强化学习 (RL)` `双足机器人` `具身智能`

* **[BPIC: 偏置并联步兵底盘控制器](https://github.com/Tensor-0/rm-biased-parallel-controller)**
  针对 RoboMaster 偏置并联机构的 C++ 底层控制框架，实现了闭链运动学正逆解算器与基于 LQR/VMC 的倒立摆平衡控制器。
  `C/C++` `运动学与动力学` `平衡控制`

* **[FDC: 摩擦轮飞镖发射控制系统](https://github.com/Tensor-0/friction-dart-controller)**
  摩擦轮飞镖发射时序与转速控制器，通过 PID/ADRC 实现双电机同步闭环，以有限状态机 (FSM) 管理发射流程。
  `STM32` `控制算法` `状态机`

* **[GMFS: 黄金矿工全栈机器人方案](https://github.com/Tensor-0/goldminer-robot-fullstack)**
  自主检索机器人系统，集成了 OpenCV 视觉检测、机械臂抓取控制与底盘驱动。
  `全栈开发` `机器视觉`
---

<a name="english-version"></a>
##  English Version

###  About Me

I study Robotics Engineering with a focus on **Embodied AI**. My work covers high-speed combat robotic systems and high-DOF bipedal locomotion, with current emphasis on **Reinforcement Learning (RL)** for sim-to-real transfer of articulated robots and robust dynamic gait generation.

*Open to collaborations on open-source robotics, RL algorithms, and related technical work.*

###  Featured Research & Projects

* **[RooCode Plus — Multi-Model Local Proxy Adapter](https://github.com/Tensor-0/roocode-plus)**
  A local proxy adapter for Roo Code, built on FastAPI to intercept and restructure HTTP requests. Dynamically injects missing fields to resolve API format incompatibilities and context truncation between Roo Code and models like DeepSeek. Includes cross-platform automation scripts for installation and testing.
  `Python` `FastAPI` `REST API`

* **[DBRL — Damiao Bipedal Reinforcement Locomotion](https://github.com/Tensor-0/dbrl-damiao-bipedal-rl)**
  RL-based gait optimization framework for the Damiao 19-DOF bipedal humanoid robot. Covers Sim-to-Real deployment and high-DOF policy control on NVIDIA Orin platforms.
  `Reinforcement Learning` `Isaac Gym` `Sim-to-Real`

* **[BPIC — Biased Parallel Infantry Controller](https://github.com/Tensor-0/rm-biased-parallel-controller)**
  C++ motion control framework for RoboMaster biased parallel infantry chassis. Implements non-linear kinematics solvers and LQR/VMC balance control.
  `C++` `Kinematics` `LQR/VMC`

* **[FDC — Friction Dart Controller](https://github.com/Tensor-0/friction-dart-controller)**
  Launch sequence controller for friction-wheel dart systems, with dual-motor speed synchronization (PID/ADRC) and finite-state-machine sequencing.
  `Control Theory` `Embedded Systems`

* **[GMFS — GoldMiner Full-Stack](https://github.com/Tensor-0/goldminer-robot-fullstack)**
  Full-stack autonomous retrieval system integrating OpenCV-based object detection with STM32 chassis control.
  `STM32` `Computer Vision` `Full-Stack`

---

###  全栈技术储备 (Technical Stack)

** 算法与仿真 (AI & Simulation)**
<p>
  <img src="https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white">
  <img src="https://img.shields.io/badge/Isaac_Gym-76B900?style=for-the-badge&logo=nvidia&logoColor=white">
  <img src="https://img.shields.io/badge/MuJoCo-000000?style=for-the-badge&logo=openai&logoColor=white">
  <img src="https://img.shields.io/badge/ROS2-22314E?style=for-the-badge&logo=ros&logoColor=white">
</p>

** 软件与硬件 (Software & Hardware)**
<p>
  <img src="https://img.shields.io/badge/C++-00599C?style=for-the-badge&logo=c%2B%2B&logoColor=white">
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white">
  <img src="https://img.shields.io/badge/Linux_Ubuntu-E95420?style=for-the-badge&logo=ubuntu&logoColor=white">
  <img src="https://img.shields.io/badge/STM32_/_Orin-76B900?style=for-the-badge&logo=nvidia&logoColor=white">
</p>

---

### 联系方式 (Connect with Me)

<p>
  <a href="mailto:3247167757@qq.com"><img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white"></a>
  <a href="https://space.bilibili.com/171912855"><img src="https://img.shields.io/badge/Bilibili-00A1D6?style=for-the-badge&logo=bilibili&logoColor=white"></a>
  <a href="https://www.zhihu.com/people/70-53-83-52-49"><img src="https://img.shields.io/badge/Zhihu-0084FF?style=for-the-badge&logo=zhihu&logoColor=white"></a>
</p>

---

<p align="center">
  <img src="https://github-readme-streak-stats.herokuapp.com/?user=Tensor-0&theme=radical&hide_border=true" alt="GitHub Streak" />
</p>

<p align="center">
  <i>"Iterating on the future of embodied locomotion, one tensor at a time." </i>
</p>
