# YOLOv5_missiledetection
Missile Detection Project
A YOLOv5-based passive missile detection and tracking system using simulated Solar Blind Ultraviolet (SBUV) imagery, implemented in Google Colab for DRDO’s Missile Approach Warning System (MAWS) research.

Project Overview
This repository contains code, data configuration, and results for training and evaluating a YOLOv5 model to detect missile plume signatures in simulated SBUV images. The system achieves real-time inference (≈36 FPS) with high accuracy (95% mAP@0.5) and is designed to enhance aircraft survivability against MANPADS, SRAAMs, and WVRAAM threats.

Key Features:
1. Deep Learning Model: YOLOv5s fine-tuned on a custom missile dataset.
2. Synthetic Data: 768 annotated images (690 train, 78 validation) from Roboflow.
3. Real-Time Inference: 27.3 ms per frame on Tesla T4 (Google Colab).
4. Video Demo: Synthetic validation video for end-to-end detection.
5. Modular Pipeline: Easy extension for tracking and trajectory prediction.
6. Reproducible: Fully containerized Colab notebook and scripts.

