---
title: "Design and Control of a Robotic Ankle Prosthesis for Task Variability"
collection: talks
type: ""
permalink: 
excerpt: " **Duration:** Mar 2020 - Dec 2021 <br> **Contribution:** Embedded System Design, Data Acquisition, Machine Design, Finite State Control, EMG-Driven Neuromuscular Modeling, Control Theory, Non-Linear Optimization, Real-Time Control System Design, Design of Experiment." 
venue:  
location: 
---

## Mechanical and Embedded System Design

I contributed to the development of a robotic ankle prosthesis that restores 1 degree-of-freedom (1-DOF) motion to the user, conceptualizing and developing the embedded control system and data acquisition system to allow for real-time control and monitoring of the prosthesis. The novel design included a variable stiffness spring that allowed the user to easily adjust the stiffness and range of motion of the device, which could be adjusted by adding or removing bevel discs, or using different stiffness bevel discs, enabling it to perform a variety of tasks with optimum performance.

<div align="center">
<img src="http://cshah96.github.io/ChinmayShah.github.io/images/Combo.JPG" alt="Image not shown" width="300" height="300">
 </div>

## Finite State Machine Validation

To validate the device, I developed a simple finite state control system that broke level ground walking and stair climbing down into phases, using sensor data to monitor the state of the ankle and execute the appropriate impedance strategy for each phase. This confirmed the device and its instrumentation could support real-time, task-specific control. The results of this study were presented at [IROS 2021.](https://cshah96.github.io/ChinmayShah.github.io//publications/1-Paper/)

<div align="center">
<video width="640" height="360" controls>
  <source src="http://cshah96.github.io/ChinmayShah.github.io/images/IROS_FINAL_VIDEO.mp4" type="video/mp4">
  Your browser does not support the video tag.
</video>
</div>

## EMG-Driven Volitional Control — Master's Thesis Contribution

While the finite state controller validated the device, it remained limited to preprogrammed, cyclic tasks and could not account for user intent, making it susceptible to unknown disturbances. To address this, I developed an EMG-driven neuromuscular model-based controller for volitional control of the prosthesis, enabling the user to perform unpredictable and non-repetitive tasks. The controller uses EMG signals from the muscle to relay user intent to the device, replicating the human neuromuscular system with a virtual ankle joint model made of two hill-type muscle lumped parameter models representing the plantarflexors and dorsiflexors.

<div align="center">
<img src="http://cshah96.github.io/ChinmayShah.github.io/images/Control_Diagram.png" alt="Image not shown" width="450" height="450">
 </div>

The model was trained using EMG signals and biomechanical data collected during level ground walking at different speeds, then validated through offline simulations and human subject testing across tasks it wasn't trained for. This was the first controller of its kind implemented in real-time on a robotic prosthetic device and tested while performing unpredictable, non-repetitive tasks. The results of this study were presented at [IROS 2022.](https://cshah96.github.io/ChinmayShah.github.io//publications/2-Paper/)

<div align="center">
<video width="640" height="360" controls>
  <source src="http://cshah96.github.io/ChinmayShah.github.io/images/Dynamic_balance_crop_2.mp4" type="video/mp4">
  Your browser does not support the video tag.
</video>
</div>

<div align="center">
<video width="640" height="360" controls>
  <source src="http://cshah96.github.io/ChinmayShah.github.io/images/ICRA_2022_without_slow_motion.mp4" type="video/mp4">
  Your browser does not support the video tag.
</video>
</div>
