# 🤖 Seokhyun Hong's Robotics Portfolio

A portfolio of robotics projects including UGV, USV, and Excavator simulations and field tests. Built using ROS, Gazebo, Unity, and custom C++/Python code.

---

## 🚗 UGV Simulation  (09.2021 - 12.2021)
**Hanyang University – Dept. of Automotive Engineering Senior Project**

- Developed a differential-drive robot using URDF
- Used [sjtu_drone](https://github.com/tahsinkose/sjtu-drone) for goal tracking reference
- Implemented with **ROS Melodic**, **Gazebo**, and **C++**

### 🧩 System Overview

UGV control architecture:  
![UGV Control Diagram](images/UGV/UGV_diagram.png)

🔗 [GitHub Repository](https://github.com/amoogeona11/Reduced-path-Iterative-A-star)

---

### 🗺️ A* Path Planning

- Grid map-based A* algorithm
- Implemented in C++
- Integrated as a ROS node in Gazebo simulation

📹 [▶️ Watch Demo](https://youtu.be/fq33Nl0Rb3Q)

---

### ♻️ A* Path Reduction

- Pruned unnecessary waypoints
- Improved efficiency and smoothness
- Maintains obstacle avoidance safety

📹 [▶️ Path Reduction Video](https://youtu.be/kfxGbPY_JvY)

![Path Reduction](images/UGV/RPAstar.png)

---

### 📊 Simulation Maps & Performance

- `P_time`: A* computation time  
- `R_time`: Actual time taken to reach the goal

| Map | Comparison Table |
|-----|------------------|
| ![Map](images/UGV/Map.png) | ![Table](images/UGV/Table.png) |

---

### 🚧 Obstacle Avoidance

- Combines global A* planning with local reactive avoidance
- Supports live obstacle updates and dynamic re-planning

📹 [▶️ Watch Video](https://youtu.be/nBfN8mHjhsk)

---

## 🧠 Sensor Fusion (ESKF) (03.2022 - 12.2022)

### 📸 Camera–IMU Fusion

- **Prediction**: Integrated IMU (position, velocity, orientation)
- **Correction**: Pose estimation using **Aruco markers**
- Developed for indoor applications

📹 [▶️ Indoor Fusion Demo](https://youtu.be/gelpOx11oOY)

---

### 🛰️ GPS–IMU Fusion

- **Prediction**: Integrated IMU measurements
- **Correction**: Dual RTK-GPS readings (considering extrinsics to vehicle frame)
- Developed for outdoor autonomous vehicle control

---

## 🚤 USV Simulation & Field Test (03.2022-03.2024)

### 🧼 Lake-Cleaning USV  
**Seoul National University – Interactive & Networked Robotics Lab (Prof. Dongjun Lee)**

![USV Platform](images/USV/USV.png)

**Custom-built autonomous surface vessel:**

**System Specs:**
- Structure: Catamaran
- Size: 800 × 640 × 220 mm
- Mass: 20.66 kg
- Inertia (Iz): 1.37 kg·m²
- Materials: FRP, aluminum, 3D-printed parts

**Electronics:**
- Intel NUC (i5-8th Gen)
- Dual RTK-GPS (SMC-2000 / SMC+)
- Velodyne VLP-16 LiDAR
- Pixhawk, Diskdrive actuator, Teensy 4.0
- LTE router for remote access

**Highlights:**
- Polygon-based optimal coverage path generation
- PID-controlled velocity field following
- Validated in simulation, tested indoors, and deployed on water

📹 [Simulation Video](https://youtu.be/kfoeWoRUoZ0)  
📹 [Field Test Video](https://youtu.be/pwgTA8-aSr0)

---

### 🛠️ Fail-Safe Control Under Actuation Failure (03.2024 - 11.2024)

Developed a control strategy for one-sided actuator failure:

- Transformed dynamics into **polar coordinates** to reduce system states
- Applied **Model Predictive Control (MPC)** on reduced polar coordinate system dynamics
- Achieved improved stability and controllability

**Simulated and Real-World Results:**  
![Simulation Result](images/USV/sim.gif)  
![Real-World Result](images/USV/real.gif)

📄 Refer to [Master's Thesis](images/석사논문_홍석현.pdf) for detailed explanation

---

## 🚜 Excavator Simulation & Field Test (03.2025 - )

- Pick and place excavator Gazebo simulation
- Built automated pulper feeding framework
- Built excavator simulator in **Unity**

![Excavator Demo](./media/excavator.gif)  
📹 [▶️ Watch Full Demo](https://youtu.be/nSXMK3pkZn8)

---

> 🚀 Passionate about autonomous systems, real-world implementation, and practical robotics innovation.
