---
title: "Autonomous Delivery & Security Robots"
excerpt: "Path planning, behavior coordination, and ML-based collision avoidance for last-mile delivery and security platforms<br/>"
collection: portfolio
---

**DEKA Research and Development, Jan 2022 – Aug 2023**

## Overview

DEKA's autonomous robot programs — a last-mile delivery robot developed in partnership with FedEx, and an autonomous security platform — required navigation systems capable of handling the full complexity of real-world urban environments: crowded sidewalks, road crossings, narrow corridors, and dynamic pedestrians. As a Robotics Control Systems Engineer, the work spanned the full navigation stack from global path planning through to low-level controller integration, taking systems from concept toward market-ready deployment.

## Path Planning & Behavior Coordination

**High-Level Behavior Planner**
- Designed the behavior coordination layer that arbitrates between the global path planner and context-specific local controllers depending on environment state (sidewalk, road, intersection, indoor)
- Implemented pedestrian yielding logic using prediction-aware decision rules, ensuring socially compliant navigation

**Planning Algorithms**
- Implemented and tuned core planning algorithms: **A\*** for grid-based global planning, **RRT** for kinodynamic planning in constrained spaces, **Grassfire** for distance-field computation
- Benchmarked and selected algorithm variants appropriate for each navigation context

## Collision Avoidance

**ML-Based Trajectory Prediction**
- Engineered a hierarchical collision-check library that integrates ML-based pedestrian trajectory predictions to anticipate dynamic obstacle positions ahead of time
- Combined predicted future occupancy with conservative geometric safety margins for robust collision checking
- Achieved a **~16% reduction in collision incidents** during real-world testing compared to reactive-only baseline

## Indoor Navigation

**MPC Cost Layer Engineering**
- Introduced reachability analysis and Euclidean-distance cost layers into the Model Predictive Controller (MPC) to penalize trajectories that approach dead-ends or narrow passages in cluttered indoor environments
- Leveraged GPU-accelerated computation to maintain real-time performance at MPC update rates despite the added computational cost

## Systems Engineering

Contributed to the full development lifecycle — from algorithm prototyping in simulation (ROS + Gazebo) through hardware integration testing to real-world field trials — gaining experience with the engineering rigor required for safety-critical autonomous systems targeting commercial deployment.
