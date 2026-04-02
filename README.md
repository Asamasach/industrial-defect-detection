# Industrial Defect Detection System

Real-time defect detection system for factory production lines, deployed across 100+ industrial inspection projects.

[![Python](https://img.shields.io/badge/Python-3.8+-blue)](https://python.org)
[![C++](https://img.shields.io/badge/C++-17-orange)](https://isocpp.org)
[![ONNX](https://img.shields.io/badge/ONNX_Runtime-Inference-green)](https://onnxruntime.ai)
[![Docker](https://img.shields.io/badge/Docker-Deployed-blue)](https://docker.com)
[![Demo](https://img.shields.io/badge/HuggingFace-Live_Demo-yellow)](https://huggingface.co/spaces/smartfalcon-ai/Industrial-Defect-Detection)

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

## 3D Vision, VLM & Other Projects

Additional projects including 3D reconstruction, multi-camera calibration, vision-language model evaluation, and auto-labeling pipelines are available under NDA.

**For demos, technical details, or collaboration inquiries, please contact me directly:**
s.mahdi.sadat.hosseini@gmail.com

---

## Architecture
```
Camera Feed --> Preprocessing --> YOLO Inference --> Post-processing --> REST API / HMI
                                    (ONNX Runtime)
```

## Tech Stack
- **Inference:** YOLO (v5/v8/v11), ONNX Runtime
- **Languages:** C++, Python
- **Preprocessing:** OpenCV (adaptive filtering, morphological ops, contour analysis)
- **Deployment:** Docker, REST API, Linux
- **CI/CD:** Jenkins, Git, CMake

## Publication
Khairy, M., **Sadat Hosseini, S. M.**, Aghili, M. S. (2023). *Design and Implementation of an Intelligent Fabric Quality Control System.* Proc. 13th National Conf. on Textile Engineering, Amirkabir University, Tehran.
