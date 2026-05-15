# Max (Tensor-0)
**Robotics System Engineer | Embodied AI & Legged Locomotion**
[Zhihu](https://www.zhihu.com/people/70-53-83-52-49) | [Bilibili](https://space.bilibili.com/171912855) | [RoboMaster Forum](https://bbs.robomaster.com/user/262448)

---

## 核心定位 (Engineering Identity)
专注于复杂异构硬件架构下的高动态运动控制，与足式/双足机器人的 Sim-to-Real 物理实体部署。
擅长在极度受限的算力与物理边界下，完成从**动力学建模 (Kinematics/Dynamics)** 到**多总线实时网络 (Real-time Bus Topology)**，再到**敏捷工程交付 (Agile Commissioning)** 的全链路系统闭环。不迷信纯理论仿真，追求物理世界的极致鲁棒性。

---

## 核心工程矩阵 (Core Architecture & Projects)

### 1. 偏置并联轮腿高动态控制系统 (Biased-Parallel Legged System)
*C/C++ | LQR/VMC | STM32 H7+F407 | System Architecture*
针对非线性强耦合的偏置并联构型，从零构建的底层运动控制与硬件通信框架。
* **异构双核拓扑与总线隔离**：设计 STM32 H7+F407 分布式架构。针对高频动力学解算导致的通讯拥塞，在物理层隔离 FDCAN (关节力矩反馈) 与 CAN (低频机构)，并实施 FIFO 接收邮箱队列深度优化，保障底层硬实时性。
* **强弱电解耦与系统防御**：构建动力域与控制域隔离的旁路供电拓扑，杜绝高频急刹反电动势导致的逻辑层欠压复位 (Brownout Reset)。
* **极限状态空间整定**：建立等效二级倒立摆模型与雅可比力矩映射。基于稳态误差边界探索，完成极值姿态抗扰优先级的 LQR 状态反馈矩阵标定，实现 300mm 容差内的极致刹车防倾倒。
* **敏捷交付与联调 SOP**：引入软硬双重 E-Stop 机制与“降维正交测试”规范，剥离多输入多输出 (MIMO) 系统的耦合干涉，在恶劣资源环境下实现单原型机零严重炸机交付。

### 2. DBRL: 高自由度双足机器人 RL 部署框架 (Bipedal RL Locomotion)
*Python | Isaac Gym | Sim-to-Real | NVIDIA Orin*
针对 19-DOF 双足机器人的强化学习步态演进与物理部署流水线。
* **策略训练与域随机化**：基于 Isaac Gym 构建大规模并行物理仿真环境，设计针对电机死区、通信延迟与地面摩擦力的 Domain Randomization 策略。
* **物理端侧部署**：完成从 PyTorch 策略模型到 ONNX 的轻量化编译，打通 NVIDIA Orin 算力平台到下位机驱动器的低延迟力矩下发链路，探索高维动作空间在物理实体的端到端映射。

### 3. 本地化开发者工作流集成 (Developer Toolchains & Ops)
*Python | FastAPI | Shell | System Scripting*
* **RooCode Plus Proxy**：独立开发多模型本地代理服务。基于 FastAPI 拦截并重构 HTTP 请求，动态注入缺失字段，解决 DeepSeek V4 等模型 API 与开发工具间的格式阻断与上下文截断问题，沉淀自动化构建脚本。
* **HiMa (海马) 开源工具**：构建极简的开发者工具链集，优化个人研发效率。

---

## 武器库 (Technical Arsenal)
* **控制理论**：LQR / VMC (Virtual Model Control) / PID / ADRC / FSM (Finite State Machine)
* **具身智能**：Isaac Gym / RL Locomotion / Sim-to-Real Transfer
* **嵌入式与架构**：STM32 (H7/F407) / FDCAN / 异构总线网络 / 强弱电隔离
* **软件工程**：C/C++ / Python / Linux (Ubuntu) / API Proxy & Scripting
