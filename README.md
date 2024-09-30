# Face Emotion Detection Using YOLOv8

This project focuses on detecting facial emotions using the YOLOv8 architecture. The model is trained to identify four different classes of emotions: **angry**, **sad**, **surprised**, and **happy**. The YOLOv8 model is leveraged for its powerful object detection capabilities, enabling fast and accurate emotion detection in images and videos.

## Key Features

- **YOLOv8 Model**: Utilizes the latest version of YOLO (You Only Look Once) architecture for real-time face emotion detection.
- **Classes**: The model is trained to detect the following four classes:
  - **Angry**
  - **Sad**
  - **Surprised**
  - **Happy**
- **Custom Dataset**: The dataset is carefully labeled with four distinct emotions for robust training and evaluation.
- **Data Augmentation**: Applied augmentations like rotation, flipping, and color adjustments to improve generalization and reduce overfitting.
- **Bounding Box Predictions**: Outputs bounding boxes around faces with predicted emotion labels and confidence scores.
- **Model Training**: The training was performed using stochastic gradient descent with warm restarts and a cosine learning rate schedule for improved convergence.
- **Evaluation**: Performance metrics include precision, recall, mAP50, and mAP50-95 on a validation set.
- **Inference**: Fast inference pipeline optimized for real-time performance in live video streams.

## How to Use

To clone and run the project, follow these steps:

```bash
# Clone the repository
!git clone https://github.com/abuzarkhaaan/Face-Emotion-Detection-YOLOv8.git

# Navigate into the project directory
cd Face-Emotion-Detection-YOLOv8

# Install required dependencies
pip install -r requirements.txt

# Run inference
python detect.py --weights best.pt --source input_video.mp4

