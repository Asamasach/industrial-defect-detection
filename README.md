# Industrial Defect Detection System

Real-time defect detection system for factory production lines, deployed across 100+ industrial inspection projects.

## Live Demo
[Try it on HuggingFace](https://huggingface.co/spaces/smartfalcon-ai/Industrial-Defect-Detection)

---

## Factory Defect Detection

### Glass Defect Detection (Car Rear Glass)

<video src="assets/car-rear-glass.mp4" controls width="720"></video>

### PVB Film Inspection

<video src="assets/pvb-film.mp4" controls width="720"></video>

### Textile Defect Detection (Jean Stenter)
Real-time denim fabric inspection on stenter production line.

[Watch demo on HuggingFace](https://huggingface.co/spaces/smartfalcon-ai/Industrial-Defect-Detection)

### Bottle Inspection
Automated bottle defect detection on high-speed production line.

[Watch demo on HuggingFace](https://huggingface.co/spaces/smartfalcon-ai/Industrial-Defect-Detection)

### Pen Inspection
Surface defect detection for pen manufacturing line.

[Watch demo on HuggingFace](https://huggingface.co/spaces/smartfalcon-ai/Industrial-Defect-Detection)

---

## Shipment Detection

### Stationary Barcode Detection (YOLO)

<video src="assets/stationary-shipment-detection-barcode-yolo.mp4" controls width="720"></video>

### Stationary Object Detection

<video src="assets/stationary-shipment-detection-object.mp4" controls width="720"></video>

---

## 3D Vision & VLM

- **3D Reconstruction & Calibration:** Multi-camera calibration, lens distortion correction, coordinate frame registration for industrial inspection setups
- **Vision-Language Models:** Benchmarking VLMs (GPT-4V, Qwen-VL, LLaVA) for zero-shot industrial defect classification and grading. See [VLM Evaluation Kit](https://github.com/asamasach/vlm-evaluation-kit)

---

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
- **Textile:** fabric defect detection (holes, stains, pattern breaks)
- **Glass:** surface scratch and bubble detection
- **Automotive:** paint defect and assembly verification
- **Packaging:** label alignment and seal integrity
- **Shipment:** barcode and object detection for logistics

## Tech Stack
- **Inference:** YOLO (v5/v8/v11), ONNX Runtime
- **Languages:** C++, Python
- **Preprocessing:** OpenCV (adaptive filtering, morphological ops, contour analysis)
- **Deployment:** Docker, REST API, Linux
- **CI/CD:** Jenkins, Git, CMake

## Publication
Khairy, M., **Sadat Hosseini, S. M.**, Aghili, M. S. (2023). *Design and Implementation of an Intelligent Fabric Quality Control System.* Proc. 13th National Conf. on Textile Engineering, Amirkabir University, Tehran.
