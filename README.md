# Industrial Defect Detection System

Real-time defect detection system for factory production lines, deployed across 100+ industrial inspection projects.

## Live Demo
[Try it on HuggingFace](https://huggingface.co/spaces/smartfalcon-ai/Industrial-Defect-Detection)

## Overview
Production-grade defect detection system that runs YOLO-based object detection models on industrial camera feeds in real time. Each domain (textile, glass, automotive, packaging) uses a dedicated model with domain-specific preprocessing and post-processing.

## Architecture
```
Camera Feed --> Preprocessing --> YOLO Inference --> Post-processing --> REST API / HMI
                                    (ONNX Runtime)
```

## Features
- Real-time inference using ONNX Runtime (C++ and Python)
- Per-domain dedicated models with optimized thresholds
- REST API endpoints for each model
- Docker-based deployment with CI/CD (Jenkins, Git)
- Model evaluation: precision, recall, F1, mAP tracking
- Integrated with [Monitait.com](https://monitait.com) for live monitoring

## Domains
- Textile: fabric defect detection (holes, stains, pattern breaks)
- Glass: surface scratch and bubble detection
- Automotive: paint defect and assembly verification
- Packaging: label alignment and seal integrity

## Tech Stack
- **Inference:** YOLO (v5/v8/v11), ONNX Runtime
- **Languages:** C++, Python
- **Preprocessing:** OpenCV (adaptive filtering, morphological ops, contour analysis)
- **Deployment:** Docker, REST API, Linux
- **CI/CD:** Jenkins, Git, CMake

## Publication
Khairy, M., **Sadat Hosseini, S. M.**, Aghili, M. S. (2023). *Design and Implementation of an Intelligent Fabric Quality Control System.* Proc. 13th National Conf. on Textile Engineering, Amirkabir University, Tehran.
