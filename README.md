# Lukas Amiet — ETH Zürich · Machine Learning & AI

An overview of my machine-learning and AI coursework and projects at ETH Zürich.
The code lives in a **private repository** — most of these are graded course
projects that the courses don't allow publishing publicly. I'm happy to share
access with anyone who'd like a closer look.

> 🔒 **Code:** [`amietlukas/eth-ml-projects`](https://github.com/amietlukas/eth-ml-projects) *(private — access on request)*
> 📫 [lukas.amiet@bluewin.ch](mailto:lukas.amiet@bluewin.ch) · [linkedin.com/in/lukas-amiet](https://linkedin.com/in/lukas-amiet)

---

## Computer Vision & AI for Autonomous Cars — *ETH TRACE · 09–12.2025*

Autonomous-driving perception: 3D LiDAR object detection, point-cloud semantic
segmentation, and monocular depth estimation.

- **[`CVAIAC/object-detection-lidar/`](https://github.com/amietlukas/eth-ml-projects/tree/main/CVAIAC/object-detection-lidar)** — 3D object
  detection from LiDAR: point-cloud → camera projection with semantic labels,
  3D bounding-box visualization, and a trained detection model.
- **[`CVAIAC/image-depth-segmentation/`](https://github.com/amietlukas/eth-ml-projects/tree/main/CVAIAC/image-depth-segmentation)** —
  point-cloud semantic segmentation + monocular depth estimation.

<p>
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

*Non-ML courses worth noting — to be listed.*

## Beyond coursework

Research and project work that lives in the GitHub organizations I'm part of:

- **Robotic Systems Lab (RSL)** — reinforcement-learning work on the ANYmal quadruped.
- **NomadZ** — full-stack humanoid robotics code.
