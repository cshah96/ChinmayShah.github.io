---
title: "Phase-Conditioned Motion Forecasting"
excerpt: "DeepPhase-inspired Periodic Autoencoder for predicting lower-limb kinematics across subjects and locomotion modes<br/>"
collection: portfolio
---

**IHMC / University of West Florida, 2024–Present**

## Overview

Predicting what the body will do next — even half a step ahead — gives a wearable robot a critical advantage. Rather than reacting to movement that has already occurred, a controller armed with motion forecasts can pre-position actuators, pre-compute torques, and deliver assistance exactly when and where it's needed. This project develops a **phase-conditioned deep learning architecture** for real-time lower-limb kinematics prediction, designed to generalize across unseen subjects and locomotion modes.

## Architecture: Periodic Autoencoder

Inspired by the DeepPhase framework for character animation, we train a **Periodic Autoencoder** that learns a compact phase representation of human gait. The key insight is that locomotion — walking, running, stair climbing — is fundamentally periodic, and embedding that periodicity explicitly into the latent space yields far better generalization than vanilla sequence models.

**Encoder**
- Takes a window of multi-modal sensor signals (joint angles, IMU, insole pressure) as input
- Outputs a low-dimensional **phase vector** encoding where the user is in their gait cycle and which locomotion mode they are performing

**Decoder / Predictor**
- Conditioned on the phase vector, predicts future joint angles (hip, knee, ankle) for a configurable prediction horizon
- Architecture enables smooth, physically plausible forecasts that respect gait periodicity

**Frequency-domain Latent Space (FLD)**
- Trained on the **Georgia Tech Lower-Limb Dataset** spanning multiple subjects and locomotion modes
- Phase representation is structured in the frequency domain, enabling principled interpolation between locomotion modes

## Results

| Metric | Value |
|--------|-------|
| Joint Angle MAE (unseen subjects) | 4–8° |
| R² (unseen subjects) | > 0.75 |
| Locomotion modes generalized | Walking, Running, Stair ascent/descent, Ramp |

## Integration with Exoskeleton Control

The learned phase encoder forms the front end of the exoskeleton's perception pipeline. Phase estimates drive the **Bio-Torque controller** timing, ensuring assistive torques are applied in-phase with the user's own muscle activity. Forecasted kinematics feed into inverse dynamics estimation, enabling the controller to anticipate loading rather than respond to it.

## Publication

- C. Shah, J. Li, G. Clark, *"Real-Time Phase Conditioned Human Motion Forecasting For Wearable Robot Control"* — submitted to IROS 2026, Pittsburgh. *(Under review)*
