---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

<style>
.cv-section { margin-bottom: 1.6em; }
.cv-entry { margin-bottom: 1.1em; }
.cv-entry-header { display: flex; justify-content: space-between; align-items: baseline; flex-wrap: wrap; }
.cv-entry-header .date { color: #888; font-size: 0.88em; white-space: nowrap; margin-left: 1em; }
.cv-institution { color: #1a6091; font-weight: 600; }
.cv-degree { font-style: italic; }
.cv-gpa { color: #555; font-size: 0.9em; }
.skill-group { margin-bottom: 0.5em; }
.skill-label { font-weight: 600; color: #333; }
</style>

Education
======

<div class="cv-section">

<div class="cv-entry">
<div class="cv-entry-header">
<span class="cv-institution">Institute for Human and Machine Cognition (IHMC) / University of West Florida</span>
<span class="date">Aug 2023 – Present</span>
</div>
<div class="cv-degree">PhD in Intelligent Systems and Robotics</div>
<div class="cv-gpa">GPA: 4.0/4.0</div>
<div>Thesis: <em>Biologically-Inspired Intent-Aware Control for Hip-Knee Exoskeletons</em></div>
</div>

<div class="cv-entry">
<div class="cv-entry-header">
<span class="cv-institution">North Carolina State University</span>
<span class="date">Aug 2019 – Dec 2021</span>
</div>
<div class="cv-degree">MS (Thesis) in Mechanical Engineering</div>
<div class="cv-gpa">GPA: 4.0/4.0</div>
</div>

<div class="cv-entry">
<div class="cv-entry-header">
<span class="cv-institution">Vishwakarma Institute of Technology (VIT)</span>
<span class="date">Aug 2014 – May 2018</span>
</div>
<div class="cv-degree">B.Tech. in Mechanical Engineering</div>
<div class="cv-gpa">GPA: 9.12/10.0</div>
</div>

</div>

Research & Professional Experience
======

<div class="cv-section">

<div class="cv-entry">
<div class="cv-entry-header">
<span class="cv-institution">Institute for Human and Machine Cognition (IHMC)</span>
<span class="date">Aug 2023 – Present</span>
</div>
<strong>Research Assistant — PhD Researcher</strong>
<ul>
  <li>Developing a biologically-inspired control framework that learns how low-dimensional motor synergies map to assistive torques for hip-knee exoskeletons across locomotion modes.</li>
  <li>Trained a Phase-based Periodic Autoencoder (DeepPhase-inspired) on the Georgia Tech Lower-Limb Dataset for human motion prediction across unseen subjects (MAE 4–8°, R² > 0.75) and locomotion modes, serving as the foundation for the FLD encoder pipeline.</li>
  <li>Developed a Temporal Convolutional Neural Network for real-time inverse dynamics estimation of hip/knee torques from wearable IMU and insole signals, informing the exoskeleton Bio-Torque controller.</li>
  <li>Designed a wearable sensor suit with 7 body-mounted IMUs and 2 pressure insoles, streaming synchronized multi-modal data at 200 Hz for offline training and real-time onboard inference.</li>
  <li>Deployed TCN models for real-time inverse kinematics and inverse dynamics estimation, enabling portable, lab-free biomechanics assessment.</li>
  <li>Applied a Linear Inverted Pendulum Model for shear force estimation to enhance gravity-compensation strategies in the exoskeleton control stack.</li>
  <li>Developing custom wireless IMU modules toward a full-body suit for continuous health monitoring and remote rehabilitation assessment.</li>
</ul>
</div>

<div class="cv-entry">
<div class="cv-entry-header">
<span class="cv-institution">DEKA Research and Development</span>
<span class="date">Jan 2022 – Aug 2023</span>
</div>
<strong>Robotics Control Systems Engineer</strong>
<ul>
  <li>Contributed to the path planning stack for an autonomous last-mile delivery robot (FedEx) and an autonomous security robot, taking systems from concept toward market-ready deployment.</li>
  <li>Developed the high-level behavior planner coordinating global path generation and context-specific controllers for sidewalk, road, and intersection navigation, including pedestrian yielding; implemented A*, RRT, and Grassfire planning algorithms.</li>
  <li>Engineered a hierarchical collision-check library leveraging ML-based trajectory predictions for dynamic obstacle avoidance, reducing collision incidents by ~16% in real-world testing.</li>
  <li>Introduced reachability and Euclidean-distance cost layers into the Model Predictive Controller (MPC) for safe navigation in narrow indoor environments; leveraged GPU programming to maintain real-time performance.</li>
</ul>
</div>

<div class="cv-entry">
<div class="cv-entry-header">
<span class="cv-institution">Neuromuscular Rehabilitation Engineering Lab, NC State University</span>
<span class="date">Mar 2020 – Dec 2021</span>
</div>
<strong>Research Assistant</strong>
<ul>
  <li>Developed an EMG-driven musculoskeletal model controller for a robotic ankle prosthesis, replicating the biological neuromuscular pathway by mapping user EMG signals through a mathematical muscle model to generate volitional torque commands.</li>
  <li>Designed a 2-muscle lumped-parameter Hill-type model and implemented a non-linear optimization scheme in MATLAB for subject-specific parameter tuning, achieving >85% torque prediction accuracy.</li>
  <li>Implemented Least Squares Policy Iteration (LSPI) for adaptive gait assistance on a hip exoskeleton, reducing metabolic cost while preserving walking efficiency.</li>
</ul>
</div>

</div>

Publications
======

<ul>{% for post in site.publications reversed %}
  {% include archive-single-cv.html %}
{% endfor %}</ul>

Technical Skills
======

<div class="cv-section">
<div class="skill-group"><span class="skill-label">Software:</span> ROS, Git, MATLAB/Simulink, TwinCAT 3.1 (EtherCAT), SolidWorks, ANSYS, VICON, Nimble Physics, MuJoCo, Isaac Sim, OpenSim</div>
<div class="skill-group"><span class="skill-label">Programming:</span> C, C++, Python, Java</div>
<div class="skill-group"><span class="skill-label">Python Packages:</span> PyTorch, NumPy, SciPy, scikit-learn, pandas, Matplotlib, Plotly, TensorBoard, OpenCV, Gymnasium, Stable-Baselines3, SQLite</div>
</div>
