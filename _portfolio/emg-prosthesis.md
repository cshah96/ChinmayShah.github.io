---
title: "EMG-Driven Robotic Ankle Prosthesis"
excerpt: "Closing the neural-to-mechanical loop: volitional control of a robotic prosthesis using an EMG-driven musculoskeletal model<br/>"
collection: portfolio
---

**Neuromuscular Rehabilitation Engineering Lab, NC State University, 2020–2021**

## Overview

Amputation severs not just bone and tissue — it severs the neural loop. The residual neuromuscular system still generates commands; the muscles still contract in response to motor neuron firing; but those commands reach no mechanical end-effector. The EMG-driven prosthesis project directly targets this broken loop by re-establishing the pathway from **muscle activation → joint torque** — now implemented in silicon and steel rather than biology.

## The Neural Loop

The biological pathway from intent to ankle torque runs: *motor cortex → spinal cord → motor neurons → tibialis anterior / soleus → ankle joint*. Amputation interrupts this at the joint. Our controller reconstructs it:

1. **Surface EMG** is recorded from residual limb muscles (tibialis anterior and soleus / gastrocnemius)
2. An **EMG-to-activation** model maps raw EMG to muscle activation levels using a nonlinear transfer function
3. A **Hill-type muscle model** converts activation to muscle force using physiological force-length-velocity relationships
4. A **moment arm model** translates muscle forces into net ankle joint torque
5. The estimated torque becomes the **volitional command** to the robotic ankle actuator

## Technical Contributions

**Hill-Type Muscle Model**
- Implemented a 2-muscle lumped-parameter Hill-type model capturing active and passive force components
- Non-linear optimization in MATLAB for subject-specific parameter tuning (muscle optimal length, tendon slack length, maximum isometric force)
- Achieved >85% torque prediction accuracy validated against inverse dynamics from motion capture and force plates

**Subject-Specific Calibration**
- Developed an isometric calibration protocol to identify individual muscle parameters efficiently
- Validated model accuracy through inverse dynamics and kinematics analyses across multiple subjects and tasks

**Extension to Hip Exoskeleton**
- Implemented Least Squares Policy Iteration (LSPI) for adaptive gait assistance on a hip exoskeleton
- Demonstrated metabolic cost reduction while preserving walking efficiency, extending the biologically-grounded philosophy from prosthesis to assistive device

## Significance

This approach preserves **volitional, intuitive control** — the user thinks about moving, and the prosthesis responds proportionally to that neural intent. Unlike finite-state machine controllers that switch between pre-programmed modes, EMG-driven control is continuous and adapts naturally to variations in terrain, speed, and intent. This work laid the groundwork for the fully integrated neuromuscular control framework pursued in the PhD research at IHMC.

## Publication

- C. Shah, A. Fleming, V. Nalam, M. Liu, H. H. Huang, *"EMG-driven Musculoskeletal model for volitional control of a robotic ankle prosthesis"* — IROS 2022, Kyoto.
