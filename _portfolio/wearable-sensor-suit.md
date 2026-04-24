---
title: "Wearable Sensor Suit"
excerpt: "Portable multi-modal sensing platform for real-time biomechanics, health monitoring, and exoskeleton control<br/>"
collection: portfolio
---

**IHMC / University of West Florida, 2023–Present**

## Overview

Clinical biomechanics labs provide gold-standard motion analysis — but only within four walls, for an hour, under artificial conditions. Real human health plays out over days, weeks, and years of continuous movement: the morning gait that reveals early Parkinson's progression, the factory shift that accumulates joint micro-damage, the post-stroke recovery session that happens far from the hospital. The **Wearable Sensor Suit** is designed to bring rigorous biomechanical measurement into those everyday contexts.

The platform integrates **7 body-mounted IMUs** and **2 plantar pressure insoles** into a lightweight, portable suit that decouples sensing from actuation. By separating the measurement system from the robotic hardware, the suit captures unbiased movement — users move naturally, without the mechanical constraint of a powered device. This makes it a versatile tool for:
- **Offline training data collection** for machine learning models
- **Real-time onboard inference** (kinematics and dynamics) during exoskeleton control
- **Continuous health and wellness monitoring** outside the lab

## Technical Architecture

**Hardware**
- 7 IMUs placed at: pelvis, bilateral thighs, shanks, and feet
- 2 plantar pressure insoles providing ground reaction force distribution and center of pressure
- Synchronized multi-modal data streaming at **200 Hz**

**Onboard Inference**
- Temporal Convolutional Network (TCN) models deployed for real-time **inverse kinematics (IK)** and **inverse dynamics (ID)** estimation — joint angles and torques computed from raw sensor streams without camera-based or force-plate infrastructure
- Enables portable, lab-free biomechanics assessment

**Future Development**
- Custom wireless IMU modules are in development to eliminate wiring constraints, extending the platform toward a full-body or modular joint-specific configuration
- Working toward **subject-specific biomechanical digital twins**: personalized models updated continuously from sensor data, supporting:
  - Out-of-lab gait analysis
  - Remote rehabilitation monitoring
  - Early assessment of neurological and musculoskeletal impairments (Parkinson's, post-stroke gait asymmetry, ACL recovery)

## Motivation: Continuous Health Intelligence

The long-term vision is a sensor suit that functions as a **continuous health observer** — detecting subtle changes in gait biomechanics before they manifest as clinical symptoms. This bridges the gap between episodic clinical assessment and the lived reality of patient recovery and aging. Combined with exoskeleton integration, the same suit that monitors can also intervene: delivering targeted assistance when effort or loading exceeds safe thresholds.
