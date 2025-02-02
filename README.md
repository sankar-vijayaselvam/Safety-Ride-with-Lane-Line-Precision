# Safety-Ride-with-Lane-Line-Precision

Project Description

This project introduces a state-of-the-art framework employing deep learning techniques to assess the risk involved in lane-changing maneuvers. Traditional methods often struggle due to reliance on expensive sensor setups and complex processing pipelines. To address these challenges, this approach utilizes deep learning algorithms to analyze short video clips captured by a single camera, making the process more accessible and reliable.

Purpose

The purpose of this framework is to:
Provide an efficient and reliable method for lane change risk assessment.
Reduce dependency on expensive sensor systems.
Leverage deep learning to extract meaningful insights from video data.

Key Insights

Mask RCNN for Semantic Segmentation: A pre-trained Mask RCNN model is employed to generate semantic segmentation masks from individual video frames, providing detailed object and spatial relationship information.

Time-Distributed CNN-LSTM Architecture: The masked frames are processed using a time-distributed CNN combined with Long Short-Term Memory (LSTM) units, capturing both spatial and temporal features effectively.

Annotated Risk Dataset: A carefully curated dataset with risk labels for semi-naturalistic lane changes enables the model to learn complex risk patterns.

Optimized Network Architecture: Extensive experiments were conducted to evaluate various state-of-the-art architectures, leading to an optimized layout and training strategy.

High Performance: The proposed framework achieved an impressive Area Under the Curve (AUC) score of 0.937 in risk assessment.

Dataset Details

The dataset used in this framework includes:
Annotated Video Clips: Short video sequences of lane-changing maneuvers with risk labels.
Semantic Segmentation Masks: Generated using Mask RCNN for detailed scene understanding.
Training and Validation Splits: Ensuring robust model generalization.

How to Use

Install required dependencies.
Load the dataset and pre-trained Mask RCNN model.
Process video frames to generate segmentation masks.
Train the CNN-LSTM model using annotated data.
Evaluate the framework using test data and analyze the risk predictions.

Prerequisites

Python 3.x
TensorFlow / PyTorch
OpenCV
Pre-trained Mask RCNN model

Future Enhancements

Integration with real-time vehicle monitoring systems.
Expansion of the dataset to include diverse driving conditions.
Improvement of the model's explainability and interpretability.
