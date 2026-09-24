---
permalink: /
title: ""
excerpt: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
feature_row:
  - title: "Real-Time Phase-Conditioned Human Motion Forecasting <br><small>IROS 2026</small>"
    video: "IROS_2026_Chinmay_Video_Submission_Mar_5.mp4"
    url: "/talks/4.3-Real-Time%20Human%20Motion%20Forecasting/"
  - title: "EMG-Driven Volitional Control of a Robotic Ankle Prosthesis <br><small>IROS 2022</small>"
    video: "ICRA_2022_without_slow_motion.mp4"
    url: "/talks/4-Robotic%20Ankle%20Prosthesis/"
  - title: "Dynamic Balance Recovery"
    video: "Dynamic_balance_crop_2.mp4"
    excerpt: >
      Robotic ankle prosthesis recovering balance under an unexpected disturbance, controlled by the EMG-driven volitional controller.
    url: "/talks/4-Robotic%20Ankle%20Prosthesis/"
  - title: "BAJA SAE Off-Road Vehicle"
    video: "WOQD9547.MP4"
    excerpt: >
      The off-road vehicle I helped design and build as Captain and Technical Head of Powertrain Systems for the BAJA SAE team.
    url: "/talks/CVTProjects"
---

I’m a Robotics PhD student at the Institute for Human & Machine Cognition ([IHMC](https://robots.ihmc.us/)), where I study how human motion can be understood, predicted, and translated into intelligent robotic assistance. My long-term goal is to develop intuitive exoskeletons that adapt to each user across a wide range of movements and feel natural to wear.

My research focuses on **intent-aware representations of human motion for proactive exoskeleton assistance**. Building on latent motion models such as DeepPhase and Fourier Latent Dynamics (FLD), I learn continuous, phase-structured representations of human movement directly from motion and biomechanics data. This *phase manifold* captures where a person is in a movement and where they are headed, across users, activities, and transitions.

My current work explores **phase-manifold-driven torque shaping**—using this learned representation to shape exoskeleton assistance. Instead of mapping sensor measurements directly to torque, the controller reasons about the user’s position and progression on the manifold, enabling smooth, proactive impedance-based assistance and recognition of unfamiliar motions. Through a teacher–student framework, representations learned from lab-grade biomechanics are distilled into models that run in real time using a small set of wearable IMUs.

I also develop wearable sensing platforms for collecting motion data beyond the lab. My broader work spans IMU-based sensing, inverse dynamics estimation, intent prediction, and human-in-the-loop control, with applications in assistive robotics, rehabilitation, and digital human modeling.

Before IHMC, I was a Robotics Control Systems Engineer at DEKA Research & Development, where I developed planning and control software for autonomous mobile robots. Earlier, I was a Research Assistant in the Neuromuscular and Rehabilitation Engineering Lab at NC State University, working on EMG-driven control of powered ankle prostheses.

Outside the lab, I enjoy running, hiking, mountain biking, skiing, and cooking.

## Featured Work

{% include feature_row type="stacked" %}
