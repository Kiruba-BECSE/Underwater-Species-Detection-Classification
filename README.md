🐠 Underwater Species Detection & Classification
📌 Project Overview

This project presents an end-to-end deep learning pipeline for automated detection, tracking, and classification of underwater species from video data. The system is designed to identify fish and coral species in real-world underwater environments where challenges such as low visibility, motion blur, lighting variation, and occlusion are common.

The solution combines object detection, feature extraction, and video-level classification to produce annotated output videos with bounding boxes, class labels, confidence scores, and persistent object tracking.

🎯 Key Objectives

Detect underwater species accurately from raw video streams

Classify detected objects into species-level categories

Maintain object identity across frames using tracking

Generate an annotated output video for visual validation

Design a scalable pipeline that supports adding new species

🧠 Methodology & Workflow
1️⃣ Data Preparation

Collected underwater videos and image datasets

Extracted frames from videos and manually annotated species

Organized datasets into train / validation / test splits

Augmented data to handle class imbalance and underwater distortions

2️⃣ Object Detection (YOLO)

Used YOLO (You Only Look Once) for real-time object detection

YOLO detects fish and coral regions in each video frame

Bounding boxes are generated for all detected objects

3️⃣ Feature Extraction & Classification (EfficientNet)

Cropped detected regions are passed to EfficientNet

EfficientNet performs fine-grained species classification

Chosen for its compound scaling, high accuracy, and efficiency

Suitable for limited datasets and video-based inference

4️⃣ Tracking & Video Processing

Integrated object tracking to assign unique IDs across frames

Ensures consistent labeling of the same species throughout the video

Implemented using OpenCV-based tracking techniques

5️⃣ Output Generation

Generated annotated output videos containing:

Bounding boxes

Species names

Confidence scores

Object IDs

Saved outputs for qualitative evaluation and presentation

🛠️ Technologies Used

YOLO – Object Detection

EfficientNet – Feature Extraction & Classification

TensorFlow / Keras – Model Training & Inference

OpenCV – Video Processing & Tracking

Python – Core Development

📊 Evaluation & Validation

Evaluated model performance using:

Precision, Recall, F1-score

Confusion Matrix

Visual validation through annotated video outputs

🚀 Key Highlights

Handles real-world underwater challenges effectively

Modular pipeline (easy to add new species)

Optimized for video-based inference

Combines detection, classification, and tracking in one system

🔮 Future Enhancements

Expand to larger multi-species datasets

Improve tracking with DeepSORT

Deploy as a real-time monitoring system

Integrate with mobile or web-based dashboards


Developed as part of an advanced deep learning and computer vision project focused on marine ecosystem analysis.
