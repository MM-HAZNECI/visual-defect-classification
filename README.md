
# Visual Defect Classification

## Project Overview

Visual Defect Classification is an end-to-end Machine Learning and MLOps project focused on automated quality inspection of industrial metal surfaces.

The objective is to develop a system that classifies metal surface images into two categories:

- **Normal:** Metal surfaces without visible defects.
- **Defective:** Metal surfaces containing visible defects.

The system will support batch image processing, allowing users to upload multiple images and receive individual classification results.

## Project Objectives

- Explore and analyze industrial metal surface images.
- Develop a consistent image preprocessing and feature extraction pipeline using OpenCV.
- Train and evaluate classical Machine Learning models.
- Track experiments, metrics, and model versions using MLflow.
- Develop a REST API using FastAPI for batch image classification.
- Implement automated testing and reproducible development workflows.
- Package the application using Docker.

## Planned Technology Stack

| Category | Technology |
|----------|------------|
| Programming Language | Python |
| Computer Vision | OpenCV |
| Machine Learning | Scikit-learn |
| Experiment Tracking | MLflow |
| Backend API | FastAPI |
| Data Validation | Pydantic |
| Testing | pytest |
| Containerization | Docker |
| Version Control | Git / GitHub |
| CI | GitHub Actions |

> The architecture and technologies may be refined during development.

## Dataset

**Name:** Metal Surface Defect Dataset v1

**Source:** [Hugging Face Dataset](https://huggingface.co/datasets/rltjr/metal-surface-defect-v1)

**Original Source:** [Roboflow Universe](https://universe.roboflow.com/msdd/msdd-prompt-learning-qjz4o/dataset/9)

**License:** Creative Commons Attribution 4.0 International (CC BY 4.0)

The dataset contains industrial metal surface images labeled for defect inspection.

Dataset files will not be stored in this GitHub repository. Dataset access and preparation instructions will be documented separately.

## Planned System Architecture

The system will separate model training from model inference.

### Training Pipeline

Dataset → Image Preprocessing → Feature Extraction → Model Training → Evaluation → MLflow

### Inference Pipeline

Batch Image Upload → FastAPI → Image Validation → Preprocessing → Feature Extraction → Trained Model → Classification Results

The training and inference components will share the same preprocessing and feature extraction logic to maintain consistency.

## Model Evaluation

Model performance will be evaluated using:

- Accuracy
- Precision
- Recall
- F1-score
- Confusion Matrix
- Cross-Validation

## Development Status

**Status:** Initial development — Repository setup.

The project is currently in the setup phase. Model training, API development, and deployment have not yet been completed.

## License and Attribution

The dataset is provided by its respective creators under the CC BY 4.0 license. The dataset license does not automatically determine the license of this project's source code.

Source code licensing will be defined separately.
