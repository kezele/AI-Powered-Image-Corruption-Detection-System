# AI-Powered-Image-Corruption-Detection-System
Designed an AI-powered computer vision system for detecting and classifying image corruption types using a scalable ML inference architecture.

The system uses transfer learning with a pretrained ResNet model, synthetic corruption generation pipelines, API-based inference workflows, and deployment-oriented benchmarking to simulate a production-ready image quality analysis platform.

This project focuses not only on model accuracy, but also on:

- AI systems architecture,
- deployment design,
- inference scalability,
- benchmarking,
- and future optimization strategy.

Problem Statement

Images transmitted through storage systems, networks, cameras, or compression pipelines may become corrupted in ways that reduce usability and visual quality.

The goal of this system is to:

- detect corruption automatically,
- classify corruption type,
- support scalable inference workflows,
- and provide a foundation for future automated image repair recommendations.

Corruption Classes

| Class                | Description                         |
| -------------------- | ----------------------------------- |
| clean                | Original unmodified image           |
| blur                 | Edge/detail degradation             |
| noise                | Random pixel-level interference     |
| compression_artifact | Block/fidelity degradation          |
| color_distortion     | Color balance/coherence degradation |
| missing_block        | Spatial information loss            |

Dataset Strategy

The system uses a public clean image dataset, combined with synthetic corruption generation.

Each corruption type is generated independently to:

- reduce label ambiguity,
- improve isolated feature learning,
- and simplify model convergence during training.

Future roadmap:

- multi-label corruption detection,
- real-world corrupted image fine-tuning,
- localized corruption segmentation.

Model Strategy

The system uses transfer learning with a pretrained ResNet architecture.

Why ResNet:

- strong computer vision baseline,
- preserved low-level image features through skip connections,
- faster convergence,
- realistic production deployment workflow.

Future model comparisons:

- MobileNetV2
- EfficientNet
- Vision Transformers (ViTs)

Optimization Roadmap

Planned deployment optimizations:

- API-Level Optimization
- async processing
- request batching
- queueing

Model-Level Optimization
- ONNX export
- FP16 inference
- quantization
- pruning
  
Hardware-Level Optimization
- GPU benchmarking
- AMD ROCm compatibility testing

Tech Stack

| Category          | Tools            |
| ----------------- | ---------------- |
| Computer Vision   | OpenCV           |
| ML Framework      | PyTorch          |
| Transfer Learning | ResNet           |
| API Backend       | FastAPI          |
| Data Processing   | NumPy            |
| Benchmarking      | PyTorch profiler |
| Visualization     | Matplotlib       |
| Environment       | Python           |

