---
permalink: /
title: "About"
excerpt: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

<style>
.project-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
  gap: 1.1em;
  margin-top: 1.8em;
  margin-bottom: 0.5em;
}
.project-card {
  display: block;
  text-decoration: none !important;
  color: inherit;
  border: 1px solid #d0dce8;
  border-radius: 8px;
  padding: 1.1em 1.3em;
  background: #f5f8fc;
  transition: box-shadow 0.18s, border-color 0.18s, transform 0.18s;
}
.project-card:hover {
  box-shadow: 0 4px 16px rgba(26,70,110,0.13);
  border-color: #1a6091;
  transform: translateY(-2px);
  text-decoration: none !important;
}
.project-card h4 {
  margin: 0 0 0.45em 0;
  font-size: 0.98em;
  color: #1a6091;
}
.project-card p {
  margin: 0;
  font-size: 0.85em;
  color: #555;
  line-height: 1.5;
}
.project-card .card-tag {
  display: inline-block;
  margin-top: 0.6em;
  font-size: 0.75em;
  color: #888;
  font-style: italic;
}
.section-divider {
  border: none;
  border-top: 2px solid #e0e8f0;
  margin: 1.8em 0 1.4em 0;
}
</style>

I am a PhD researcher in Intelligent Systems and Robotics at the [Institute for Human and Machine Cognition (IHMC)](https://www.ihmc.us/) / University of West Florida, where I focus on the intersection of wearable sensing, machine learning, and exoskeleton control. My work is driven by a core question: *can we give the human body a continuous, intelligent observer — one that understands movement intent, detects early signs of dysfunction, and seamlessly augments physical capability?*

**Mission.** At its heart, my research aims to close the gap between the human neuromuscular system and robotic assistance. Injury, neurological impairment, or simple fatigue disrupts the body's finely-tuned movement patterns. My goal is to build systems that sense this disruption in real-time — through wearable IMUs, pressure insoles, and EMG — and respond by providing precisely calibrated support through exoskeletons and prostheses. This vision spans from **continuous health and wellness monitoring** (out-of-lab gait analysis, early detection of musculoskeletal and neurological impairments) to **active rehabilitation** (exoskeleton-assisted recovery after stroke or injury) and **injury prevention** (reducing joint loading and effort during demanding tasks).

**Approach.** I develop biologically-grounded control frameworks that learn from human movement. Rather than hand-crafting robot behaviors, I train deep neural networks on biomechanical signals to estimate motion intent, predict future kinematics, and compute joint torques in real time. These models run on portable, wearable platforms — decoupled from lab infrastructure — enabling the kind of naturalistic, continuous monitoring that clinical and field deployments demand.

<hr class="section-divider">

## Research Interests

- **Wearable Biomechanics** — multi-modal sensor fusion (IMU, EMG, pressure insoles) for portable motion analysis
- **Exoskeleton & Prosthesis Control** — biologically-inspired, intent-aware controllers for lower-limb rehabilitation and assistance
- **Human Motion Forecasting** — phase-conditioned deep learning for predicting gait across locomotion modes and subjects
- **Digital Twins for Rehabilitation** — subject-specific biomechanical models enabling remote health monitoring and early impairment detection

<hr class="section-divider">

## Projects

<div class="project-grid">

  <a class="project-card" href="/portfolio/exoskeleton-control/">
    <h4>Hip-Knee Exoskeleton Control</h4>
    <p>Biologically-inspired, intent-aware control for lower-limb exoskeletons using motor synergies, inverse dynamics, and phase-based motion prediction.</p>
    <span class="card-tag">PhD Thesis &bull; IHMC &bull; 2023&ndash;Present</span>
  </a>

  <a class="project-card" href="/portfolio/wearable-sensor-suit/">
    <h4>Wearable Sensor Suit</h4>
    <p>Portable multi-modal sensing platform (7 IMUs + 2 pressure insoles + EMG) for real-time biomechanics, health monitoring, and exoskeleton control.</p>
    <span class="card-tag">Hardware &bull; IHMC &bull; 2023&ndash;Present</span>
  </a>

  <a class="project-card" href="/portfolio/periodic-autoencoder/">
    <h4>Phase-Conditioned Motion Forecasting</h4>
    <p>DeepPhase-inspired Periodic Autoencoder for predicting lower-limb kinematics across subjects and locomotion modes — IROS 2026.</p>
    <span class="card-tag">Deep Learning &bull; IHMC &bull; 2024&ndash;Present</span>
  </a>

  <a class="project-card" href="/portfolio/emg-prosthesis/">
    <h4>EMG-Driven Robotic Prosthesis</h4>
    <p>Closing the neural-to-mechanical loop: volitional control of a robotic ankle prosthesis using an EMG-driven musculoskeletal model — IROS 2022.</p>
    <span class="card-tag">Prosthetics &bull; NC State &bull; 2020&ndash;2021</span>
  </a>

  <a class="project-card" href="/portfolio/autonomous-robot/">
    <h4>Autonomous Delivery &amp; Security Robots</h4>
    <p>Path planning, behavior coordination, and ML-based collision avoidance for last-mile delivery (FedEx) and autonomous security platforms.</p>
    <span class="card-tag">Autonomy &bull; DEKA R&amp;D &bull; 2022&ndash;2023</span>
  </a>

</div>
