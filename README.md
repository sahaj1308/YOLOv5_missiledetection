# YOLOv5_missiledetection
Missile Detection Project
A YOLOv5-based passive missile detection and tracking system using simulated Solar Blind Ultraviolet (SBUV) imagery, implemented in Google Colab for DRDO’s Missile Approach Warning System (MAWS) research.

Project Overview
This repository contains code, data configuration, and results for training and evaluating a YOLOv5 model to detect missile plume signatures in simulated SBUV images. The system achieves real-time inference (≈36 FPS) with high accuracy (95% mAP@0.5) and is designed to enhance aircraft survivability against MANPADS, SRAAMs, and WVRAAM threats.

Key Features
Deep Learning Model: YOLOv5s fine-tuned on a custom missile dataset.

Synthetic Data: 768 annotated images (690 train, 78 validation) from Roboflow.

Real-Time Inference: 27.3 ms per frame on Tesla T4 (Google Colab).

Video Demo: Synthetic validation video for end-to-end detection.

Modular Pipeline: Easy extension for tracking and trajectory prediction.

Reproducible: Fully containerized Colab notebook and scripts.

Repository Structure
├── README.md
├── missile_validation_video.mp4  // Synthetic demo video
├── data/
│ └── missile_data.yaml        // Data config for YOLOv5
├── models/
│ └── best.pt                 // Trained weights
├── runs/
│ ├── train/                // Training logs and metrics
│ └── detect/                // Inference outputs
├── sample_images/              // A few validation images
├── sample_labels/             // Corresponding labels
└── scripts/
├── create_video.py        // Stitch images into MP4
├── analyze_performance.py  // Plot training metrics
└── detect_video.sh        // Shell script for video inference
