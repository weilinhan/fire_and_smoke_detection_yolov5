# Fire and Smoke Detection with YOLOv5 🔥💨

This project implements **fire and smoke detection** using [YOLOv5](https://github.com/ultralytics/yolov5).  
It can be applied in early fire warning systems, warehouse safety monitoring, and indoor surveillance.  

---

## 🚀 Features
- Based on **YOLOv5** object detection framework  
- Supports **real-time fire and smoke detection**  
- Works on **images / videos / webcam streams**  
- Can be retrained with a custom dataset  

---

## 📂 Project Structure
  fire_and_smoke_detection_yolov5/
  ├── data/ # Dataset configs
  ├── models/ # Model definitions (weights not included)
  ├── runs/ # Training & inference results (ignored by .gitignore)
  ├── yolov5/ # YOLOv5 source code
  ├── requirements.txt # Python dependencies
  └── README.md # Project description

## 🔧 Requirements
    - Python >= 3.7.1  
    - PyTorch >= 1.8  
    - Other dependencies listed in `requirements.txt`  

    Install them with:  
     ```bash
      pip install -r requirements.txt

## 📥 Trained Model

  The trained YOLOv5 model is saved at:
    ```bash
    runs/train/exp30/weights/best.pt

## 🖼️ Usage
1. Inference (detect on image or video)
    ```bash
    python detect.py --weights runs/train/exp30/weights/best.pt --source 0
2. Training (if you want to retrain)
    ```bash 
    python train.py --img 640 --batch 16 --epochs 50 --data data/fire_smoke.yaml --weights yolov5s.pt --device 0
## 📊 Example Results
Here is an example of the model detecting fire:

![Fire detection result](fire_detect.jpg)



