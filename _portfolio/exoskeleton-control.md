---
title: "Hip-Knee Exoskeleton Control"
excerpt: "Biologically-inspired, intent-aware control for lower-limb rehabilitation and human augmentation<br/>"
collection: portfolio
---

**PhD Thesis Project — IHMC / University of West Florida, 2023–Present**

## Overview

The central challenge in exoskeleton control is translating subtle, continuous neural intent into the right assistive force at the right time. Assistive torques applied out-of-phase with the user's own muscle effort can cause discomfort, disturb natural gait patterns, and even increase metabolic cost — the opposite of what rehabilitation demands. This project develops a **biologically-inspired, intent-aware control framework** for hip-knee exoskeletons that estimates user intent from multi-modal wearable signals and delivers torques synchronized with the user's own neuromuscular activity.

## Key Technical Contributions

**Phase-Conditioned Motion Forecasting**
- Trained a Periodic Autoencoder (DeepPhase-inspired) on the Georgia Tech Lower-Limb Dataset for continuous gait phase estimation and joint angle prediction across unseen subjects and locomotion modes.
- Achieved MAE of 4–8° and R² > 0.75 on held-out subjects, enabling the exoskeleton to anticipate joint trajectories rather than react to them.

**Real-Time Inverse Dynamics via TCN**
- Developed a Temporal Convolutional Neural Network (TCN) that estimates hip and knee joint torques in real time from wearable IMU and pressure insole signals.
- Trained and validated on open biomechanics datasets; deployed on embedded hardware for onboard inference at control rates compatible with exoskeleton actuation loops.

**Bio-Torque Controller**
- The estimated torques feed a Bio-Torque controller that maps predicted biological joint moments to actuator commands, providing assistance proportional to and synchronized with the user's own effort.
- Integrated a Linear Inverted Pendulum Model for shear force and gravity-compensation estimation, improving controller robustness during stance and push-off phases.

**Motor Synergy Learning**
- Investigating how low-dimensional motor synergies — linear combinations of muscle activation patterns — can provide compact representations of locomotion intent, enabling generalization across tasks with fewer labeled samples.

## Platform

The control framework runs on a custom wearable sensor suit (see [Wearable Sensor Suit](/portfolio/wearable-sensor-suit/)) feeding signals at 200 Hz into onboard inference pipelines, with actuation commands sent to the exoskeleton via EtherCAT (TwinCAT 3.1).

## Broader Impact

Beyond rehabilitation, the same intent-detection and torque-augmentation stack addresses **injury prevention** in physically demanding occupations — reducing cumulative joint loading and muscle fatigue in workers performing repetitive lifting or prolonged walking. The underlying wearable monitoring platform is being developed toward continuous, out-of-lab **health and wellness monitoring** with applications in early detection of neurological and musculoskeletal impairments.

## Related Publication

- C. Shah, J. Li, G. Clark, *"Real-Time Phase Conditioned Human Motion Forecasting For Wearable Robot Control"* — submitted to IROS 2026, Pittsburgh.
