# Blind Assistance System

## Overview
The **Blind Assistance System** is an AI-powered application designed to help visually impaired individuals navigate their surroundings. It uses **YOLO (You Only Look Once) object detection** to identify objects in real-time and provides **audio feedback** using text-to-speech (TTS) technology.

## Features
- **Real-time object detection** using YOLOv3.
- **Distance estimation** to detected objects.
- **Voice feedback** for identified objects and proximity warnings.
- **Camera-based vision system** for continuous environment monitoring.

## Requirements
Ensure you have the following dependencies installed before running the project:

### **Python Libraries**
Install the required packages using:
```sh
pip install opencv-python numpy pyttsx3
```

### **YOLO Model Files**
Download the necessary YOLO model files:
- `yolov3.cfg`
- `yolov3.weights`
- `coco.names`

Place these files in the project directory.

## Installation & Setup
### **1. Clone the Repository**
```sh
git clone https://github.com/your-repo/blind-assistance-system.git
cd blind-assistance-system
```
### **3. Install Dependencies**
```sh
pip install -r requirements.txt  
```

### **4. Run the Application**
```sh
python detect.py
```

## How It Works
1. The program **captures video frames** from the webcam.
2. It applies **YOLO object detection** to recognize objects.
3. The system estimates the **distance** of the detected object using a predefined focal length.
4. If an object is **too close**, a warning is given via **voice feedback**.
5. The detected object and its distance are displayed on the screen.
6. The application runs continuously until the user presses **'q'** to exit.

## Customization
- Modify **`MIN_DISTANCE`** in the script to adjust the warning threshold.
- Replace **YOLOv3 model** with **YOLOv4** or **YOLOv8** for better accuracy.
- Improve speech synthesis by using **Google Text-to-Speech (gTTS)** instead of `pyttsx3`.

## Troubleshooting
### **1. ModuleNotFoundError for cv2**
Ensure OpenCV is installed inside the active virtual environment:
```sh
pip install opencv-python
```

## Future Improvements
- Implement obstacle avoidance using **depth sensors**.
- Enhance object recognition with **YOLOv8 or MobileNet SSD**.
- Develop a **mobile app** version for wider accessibility.

## License
This project is open-source and available under the **MIT License**.

## Author
Shreyansh Bhardwaj


