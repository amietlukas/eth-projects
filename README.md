# Lukas Amiet — ETH Zürich · Machine Learning & AI

An overview of my machine-learning and AI coursework and projects at ETH Zürich.
The code lives in a **private repository** — most of these are graded course
projects that the courses don't allow publishing publicly. I'm happy to share
access with anyone who'd like a closer look.

> 🔒 **Code:** [`amietlukas/eth-ml-projects`](https://github.com/amietlukas/eth-ml-projects) *(private — access on request)*
> 📫 [lukas.amiet@bluewin.ch](mailto:lukas.amiet@bluewin.ch) · [linkedin.com/in/lukas-amiet](https://linkedin.com/in/lukas-amiet)

---

## Embedded ML on Microcontrollers — *ETH PBL*

**[`embedded-vision-rc-car`](https://github.com/amietlukas/embedded-vision-rc-car)** *(public repo)* —
machine learning running **entirely on microcontrollers** for a gesture-controlled,
ball-chasing RC car. A hand-gesture classifier (STM32U5) turns camera input into
drive commands over Bluetooth; a YOLO-style ball detector runs on the STM32N6
on-chip NPU to find and chase a ball. Trained on a PC, then quantized and deployed
on-device, with quantization-aware training, pruning, and accuracy–latency–size
trade-off analysis.

## Computer Vision & AI for Autonomous Cars — *ETH TRACE · 09–12.2025*

Autonomous-driving perception: 3D LiDAR object detection, point-cloud semantic
segmentation, and monocular depth estimation.

- **[`CVAIAC/object-detection-lidar/`](https://github.com/amietlukas/eth-ml-projects/tree/main/CVAIAC/object-detection-lidar)** — 3D object
  detection from LiDAR: point-cloud → camera projection with semantic labels,
  3D bounding-box visualization, and a trained detection model.
- **[`CVAIAC/image-depth-segmentation/`](https://github.com/amietlukas/eth-ml-projects/tree/main/CVAIAC/image-depth-segmentation)** —
  point-cloud semantic segmentation + monocular depth estimation.

<p align="center">
  <img src="assets/lidar_3d_detection.png" width="55%" alt="3D vehicle detections in the LiDAR point cloud">
</p>
<p align="center">
  <img src="assets/task1_lidar_projection.png" width="46%" alt="LiDAR points projected onto the camera image, coloured by semantic label">
  &nbsp;
  <img src="assets/task2_3d_boxes.png" width="46%" alt="3D bounding boxes drawn on the camera image">
</p>

## Probabilistic Artificial Intelligence (PAI)

- **[`PAI/task0`](https://github.com/amietlukas/eth-ml-projects/tree/main/PAI/task0)** — Bayesian inference over a hypothesis space (Normal / Laplace / Student-t)
- **[`PAI/task1`](https://github.com/amietlukas/eth-ml-projects/tree/main/PAI/task1)** — Gaussian-Process regression with an asymmetric cost function
- **[`PAI/task2`](https://github.com/amietlukas/eth-ml-projects/tree/main/PAI/task2)** — Bayesian deep learning: uncertainty calibration for image classification
- **[`PAI/task3`](https://github.com/amietlukas/eth-ml-projects/tree/main/PAI/task3)** — Constrained ("safe") Bayesian Optimization with Gaussian Processes

## Computer Vision

- **[`lab01`](https://github.com/amietlukas/eth-ml-projects/tree/main/computer-vision/lab01-local-features)** — Harris corners, descriptors, matching
- **[`lab02`](https://github.com/amietlukas/eth-ml-projects/tree/main/computer-vision/lab02-model-fitting-and-sfm)** — RANSAC, two-view geometry, structure-from-motion
- **[`lab03`](https://github.com/amietlukas/eth-ml-projects/tree/main/computer-vision/lab03-deep-learning)** — MLP / CNN classifiers (2D points, MNIST, CIFAR-10)
- **[`lab04`](https://github.com/amietlukas/eth-ml-projects/tree/main/computer-vision/lab04-meanshift-segnet)** — Mean-shift clustering + SegNet segmentation
- **[`lab05`](https://github.com/amietlukas/eth-ml-projects/tree/main/computer-vision/lab05-point-tracking)** — RAFT optical flow + point tracking
- **[`lab06`](https://github.com/amietlukas/eth-ml-projects/tree/main/computer-vision/lab06-variational-autoencoder)** — Variational autoencoder on MNIST

## Introduction to Machine Learning (IML)

- **[`task1a`](https://github.com/amietlukas/eth-ml-projects/tree/main/IML/task1a)** — Ridge regression with k-fold cross-validation
- **[`task1b`](https://github.com/amietlukas/eth-ml-projects/tree/main/IML/task1b)** — Linear regression on engineered nonlinear features
- **[`task2`](https://github.com/amietlukas/eth-ml-projects/tree/main/IML/task2)** — Regression with preprocessing on tabular data
- **[`task3`](https://github.com/amietlukas/eth-ml-projects/tree/main/IML/task3)** — Image-similarity learning from triplets (transfer-learned CNN embeddings)

## Stochastics & Machine Learning

- **[`eth-mugs-finder/`](https://github.com/amietlukas/eth-ml-projects/tree/main/eth-mugs-finder)** — binary semantic segmentation of mugs
  ("ETH Mugs" dataset), PyTorch encoder–decoder.
- **[`distance-guesser/`](https://github.com/amietlukas/eth-ml-projects/tree/main/distance-guesser)** — distance regression from downsampled
  RGB image features (scikit-learn SVM + grid search).

---

## Bachelor's Thesis

**[Embedded Deep Learning for Real-Time Aerodynamic Flow Estimation on Wind-Turbine
Blades Using MEMS Pressure Sensors](https://github.com/amietlukas/eth-ml-projects/tree/main/bachelor-thesis)** — Center for Project-Based
Learning (PBL), ETH Zürich (MISTERY project). Lightweight CNNs/MLPs infer angle of
attack, wind speed, flow separation and stagnation point from 10 MEMS pressure
sensors, deployed on an STM32H5 microcontroller (MAE < 1°, 12 ms on-device
inference).

## Other relevant coursework

Foundational courses behind the projects above:

- **Estimation & control** — Recursive Estimation *(ongoing)* · Model Predictive Control *(ongoing)* · Control Systems I & II · Autonomous Mobile Robots · Robot Dynamics
- **Probability, signals & systems** — Probability & Statistics · Signals & Systems · Embedded Systems

## Beyond coursework

Research and project work in the GitHub organizations I'm part of:

### Robotic Systems Lab (RSL) — ANYmal-D solving a giant Rubik's cube
*Perception & Learning for Robotics (PLR) — completed · semester thesis — ongoing*

Teaching a quadruped (ANYmal-D) to solve a giant Rubik's cube via pedipulation:
- Reinforcement learning in **Isaac Lab / Isaac Sim** (RSL-RL) — articulated cube asset, reward shaping, curriculum, RND exploration, PPO teachers + student distillation.
- **Sim-to-real** transfer and deployment on ANYmal-D hardware, with real-world failure diagnosis and iterative policy refinement.
- Onboard cube perception: SAM-based segmentation, depth, colour classification, 6D pose estimation.

*(poster and demo video available on request)*

### NomadZ — autonomous humanoid soccer (RoboCup)
Building the software stack for fully autonomous humanoid soccer robots with **ETH NomadZ**:
- Implemented a **Kalman-filter ball-tracking** module (ROS 2).
- Improved **2D → 3D ball localization** from YOLOv8 detections.
- Work on the **Booster K1 and T1** humanoid platforms.
