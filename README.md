# 🤖 Seokhyun Hong's Robotics Portfolio

A collection of robotics projects including UGV, USV, and Excavator simulations and field tests. Built with ROS, Gazebo, Unity, and custom C++/Python code.

---

## 🚗 UGV Simulation  
**Hanyang University - Department of Automotive Engineering Senior Project**

- Developed a differential-drive robot in URDF
- Exploited [sjtu_drone](https://github.com/tahsinkose/sjtu-drone) as a goal point
- Built using ROS Melodic, Gazebo, and C++

### 🧩 System Overview

UGV control system diagram:  
![UGV Control Diagram](images/UGV/UGV_diagram.png)

🔗 [GitHub Repository](https://github.com/amoogeona11/Reduced-path-Iterative-A-star)

---

### 🗺️ A* Path Planning

**Grid map-based A* algorithm implementation**  
- Implemented in C++
- ROS node integration with Gazebo simulation

📹 [▶️ Watch video](https://youtu.be/fq33Nl0Rb3Q)

---

### ♻️ A* Path Reduction

- Reduced unnecessary waypoints
- Optimized for smoothness and efficiency
- Obstacle-aware pruning logic

📹 [▶️ Watch video](https://youtu.be/kfxGbPY_JvY)

![A* Path Reduction](images/UGV/RPAstar.png)

---

### 💻 Simulation Maps & Performance Comparison

- Process time (`P_time`): A* computation time  
- Runtime (`R_time`): Actual time robot takes to reach the goal

| Simulation Environment | Performance Table |
|------------------------|-------------------|
| ![Map](images/UGV/Map.png) | ![Table](images/UGV/Table.png) |

---

### 🚧 Obstacle Avoidance

- Combines global path planning with local obstacle avoidance  
- Dynamic re-planning with live obstacle updates

📹 [▶️ Watch video](https://youtu.be/nBfN8mHjhsk)

---

## 📱 Sensor Fusion
Exploited Error-state Kalman Filter
### Camera-IMU sensor fusion
- Prediction: IMU integration (position, velocity, orientation)
- Correction: Pose estimation using Aruco marker (position, orientaion)

**Developed for Indoor experiment**

### GPS-IMU sensor fusion
- Prediction: IMU integration (position, velocity, orientation)
- Correction: Dual RTK-GPS considering extrinsic with the USV (position)

**Developed for Outdoor experiment**

## 🚤 USV Simulation & Field Test
Unmanned surface vessel (USV) simulation and real-world testing.  

### Lake Cleaning USV

![USV Platform](images/USV/USV.png)

Custom designed and built platform
System Specifications:
- Intel Nuc: i5-8th gen
- RTK-GPS (SMC-2000/SMC+)
- Velodyne Puck (VLP-16)
- Pixhawk
- Diskdrive actuator
- Teensy 4.0

📹 [Simulation Video](https://youtu.be/kfoeWoRUoZ0)  
📹 [Field Test Video](https://youtu.be/pwgTA8-aSr0)
### Fail-safe Control of the USV with Acuation Failure
---

## 🚜 Excavator Simulation & Field Test

- Tracked excavator robot simulation in **Unity**
- Physics-based control using custom rigid-body dynamics
- Simulated force feedback and terrain interaction

![Excavator Demo](./media/excavator.gif)  
📹 [▶️ Watch full video](https://youtu.be/YOUR_VIDEO_LINK)

---

> ✨ Built with passion for autonomous systems, control, and real-world robotics challenges.
