---
permalink: /
title: ""
excerpt: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

I am a robotics PhD student at the [Institute for Human and Machine Cognition (IHMC)](https://www.ihmc.us/) in Pensacola, Florida, driven by a deep passion for building machines that move and assist the way biology does. My goal is to bridge the gap between human biomechanics and robotic control — designing systems that are not just capable, but intuitive and adaptive to the humans who use them.

## Research Direction

My research focuses on developing a **biologically-inspired control framework** that learns how low-dimensional motor synergies govern human locomotion and translates that knowledge into intelligent exoskeleton control.

At the core of this work is a **Phase-based Periodic Autoencoder** (inspired by the DeepPhase architecture), trained on the Georgia Tech Lower-Limb Dataset to predict joint kinematics across unseen subjects and locomotion modes (MAE 4–8°, R² > 0.75). This model serves as the foundation of an FLD encoder pipeline that captures the essential structure of gait cycles from high-dimensional motion data.

Alongside this, I have developed a **Temporal Convolutional Network (TCN)** for real-time inverse dynamics estimation of hip and knee torques directly from wearable IMU and pressure insole signals — providing the exoskeleton's Bio-Torque controller with continuous, user-specific torque references without lab-grade instrumentation. I have also applied a **Linear Inverted Pendulum Model** for shear force estimation to strengthen gravity-compensation strategies in the exoskeleton control stack.

To make this pipeline deployable outside a lab, I designed and built a **wearable sensor suit** integrating 7 body-mounted IMUs and 2 pressure insoles, streaming synchronized multi-modal data at 200 Hz. By decoupling sensing from actuation, the suit captures unbiased user intent and supports both offline model training and real-time onboard inference. TCN models running on the suit enable portable, lab-free inverse kinematics and inverse dynamics assessment. I am currently developing custom wireless IMU modules to eliminate wiring constraints and extend the platform toward a modular, full-body system for continuous health monitoring. The long-term vision is to leverage this suit as the foundation for **subject-specific biomechanical digital twins**, enabling out-of-lab gait analysis, remote rehabilitation monitoring, and early detection of neurological and musculoskeletal impairments.

## Background & Experience

My path to this research has been shaped by hands-on experience across robotics, mechanical engineering, and control systems. Before joining IHMC, I worked as a **Robotics Control Systems Engineer at DEKA Research and Development**, where I contributed to the path planning stack for a last-mile autonomous delivery robot and an autonomous security robot. This work spanned higher-level behavior planning, a hierarchical collision-check library using ML-based predictions, and GPU-accelerated cost layers for a Model Predictive Controller — giving me deep exposure to the full-stack challenge of deploying autonomous systems in real-world, dynamic environments.

Prior to DEKA, I was a **Research Assistant at the Neuromuscular and Rehabilitation Engineering Lab (NREL) at NC State University** under Dr. Helen Huang, where I developed embedded control systems for wearable robots. My primary project was to develop an EMG-driven volitional controller for a powered ankle prosthesis designed to restore biological function and support everyday activities for lower-limb amputees — an experience that cemented my interest in human-machine interfaces and user-adaptive control.

My foundation is in **mechanical engineering**, with over eight years of experience spanning autonomous mobile robots, wearable assistive devices, and mechanical design for automotive applications. This background in dynamics, manufacturing, and mechatronics continues to inform how I approach robotic systems — from sensor integration and actuator selection to the physical embodiment of control architectures.

Outside of research, I find balance in running, hiking, mountain biking, skiing and cooking.
