# HomeWell AI/ML Service

This repository implements a Post-LOS AI/ML service using TensorFlow 2.16 + Keras, leveraging mature GPU ops and TensorFlow Serving for inference at scale.

## Components

- **ml_service/train/**: Training pipeline using TF2.16 + Keras
- **ml_service/serve/**: Model export and TF Serving deployment
- **ml_service/client/**: Example client for inference
- **scripts/**: Data preprocessing utilities

## Prerequisites

- Docker & Docker Compose
- NVIDIA GPU drivers + NVIDIA Docker runtime
- Python 3.9+ (for training & client)


---
## 1. Training the Model

1. Build the training container:
   ```bash
   cd ml_service/train
   docker build -t homewell-ai-train:latest .
