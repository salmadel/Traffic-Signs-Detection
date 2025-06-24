# 🚦 Traffic Signs Detection 

## Project Overview
This project uses the YOLOv8 object detection model to detect and classify various traffic signs from images and videos. The system aims to support intelligent transportation systems by providing real-time, accurate recognition of traffic signs to enhance road safety and assist autonomous vehicles.

## Dataset Overview
[Dataset Link](https://www.kaggle.com/datasets/pkdarabi/cardetection)

The dataset contains labeled images of various traffic signs, including:
- Traffic lights (Green, Red)
- Stop sign
- Speed limits (10 to 120 km/h in steps of 10)

The dataset is structured in YOLO format and includes:
- `train/`, `val/`, and `test/` folders with images and annotations
- A `data.yaml` file specifying class names and paths

## Technologies & Libraries
- **Python 3.11**
- **[Ultralytics YOLOv8](https://github.com/ultralytics/ultralytics)**
- **OpenCV**
- **Matplotlib**
- **NumPy**

## Project Workflow
1. **Setup & Installations**:
  Install Ultralytics and import necessary libraries.

2. **Model Training**:
   The YOLOv8s model was trained on a custom dataset for 50 epochs, using images resized to 640 pixels and a batch size of 16. The training configuration was specified in the data.yaml file.
   
3. **Evaluation**: Measured precision, recall, mAP@0.5, and mAP@0.5:0.95:
   - Confusion Matrix
   - PR & F1 Score Curves
   - Per-class mAP bar chart

4. **Inference**:
   - Detected traffic signs in random test images
   - Drew bounding boxes with class labels and confidence scores
   - Ran the model on a video file and saved the annotated output

## Results
YOLOv8s Model Evaluation Metrics:
- **Precision**: 96.5%
- **Recall**: 93.6%
- **mAP@0.5**: 97.2%
- **mAP@0.5:0.95**: 85.5%

## Model Inference
- **Random Images**:

![__results___7_0](https://github.com/user-attachments/assets/aef0ad78-ad2f-4d74-be07-ba9c375d40c3)

- **Video**:

https://github.com/user-attachments/assets/49212acd-1808-453e-947e-89f25803f7a6






