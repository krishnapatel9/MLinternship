Week 10: YOLOv8 Object Detection — Key Concepts

focus on building a complete object detection pipeline using Ultralytics YOLOv8 — from setup to model evaluation.
The goal is to understand how modern computer vision models detect and localize objects in images.

1. Understanding YOLOv8
YOLO (You Only Look Once) is a deep learning model for real-time object detection.
YOLOv8, the latest version by Ultralytics, improves accuracy, speed, and flexibility for custom datasets.
Core idea: a single neural network predicts bounding boxes and class labels directly from images.

2. Dataset Creation & Annotation
Object detection requires labeled data with bounding boxes around objects.
Roboflow was used to:
Upload or import image datasets.
Annotate objects manually.
Export datasets in YOLOv8 format (ready for training).
Typical dataset size: 50–100 images of simple objects (e.g., pens, cups, or masks).

3. Model Training
The YOLOv8 model was trained on the annotated dataset using configuration files (data.yaml).
Key training parameters:
Epochs – total training cycles.
Image size (imgsz) – resolution for model input.
Batch size – number of images processed together.
The model learns to identify and localize objects from the labeled images.

4. Model Evaluation
The model’s accuracy was assessed using mAP (mean Average Precision) — a standard metric in object detection.
Evaluation also involved testing on unseen images to visualize bounding boxes and confidence scores.
Results highlight how well the model generalizes to new data.


