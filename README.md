
<div align="center">

# YOLOv8 Streamlit APP

## Introduction
This repository supply a user-friendly interactive interface for [YOLOv8](https://github.com/ultralytics/ultralytics) and the interface is powered by [Streamlit](https://github.com/streamlit/streamlit). It could serve as a resource for future reference while working on your own projects.

## Features
- Feature1: Object detection task.
- Feature2: Multiple detection models. `yolov8n`, `yolov8s`, `yolov8m`, `yolov8l`, `yolov8x`
- Feature3: Multiple input formats. `Image`, `Video`, `Webcam`

## Interactive Interface
### Image Input Interface
![image_input_demo](https://github.com/JackDance/YOLOv8-streamlit-app/blob/master/pic_bed/image_input_demo.png)

### Video Input Interface
![video_input_demo](https://github.com/JackDance/YOLOv8-streamlit-app/blob/master/pic_bed/video_input_demo.png)

### Webcam Input Interface
![webcam_input_demo](https://github.com/JackDance/YOLOv8-streamlit-app/blob/master/pic_bed/webcam_input_demo.png)


## Installation
### Create a new conda environment
```commandline
# create
conda create -n yolov8-streamlit python=3.8 -y

# activate
conda activate yolov8-streamlit
```
### get the pro

### Install packages
```commandline
# yolov8 dependencies
pip install ultralytics

# Streamlit dependencies
pip install streamlit
```
### Download Pre-trained YOLOv8 Detection Weights
Create a directory named `weights` and create a subdirectory named `detection` and save the downloaded YOLOv8 object detection weights inside this directory. The weight files can be downloaded from the table below.

| Model                                                                                | size<br><sup>(pixels) | mAP<sup>val<br>50-95 | Speed<br><sup>CPU ONNX<br>(ms) | Speed<br><sup>A100 TensorRT<br>(ms) | params<br><sup>(M) | FLOPs<br><sup>(B) |
| ------------------------------------------------------------------------------------ | --------------------- | -------------------- | ------------------------------ | ----------------------------------- | ------------------ | ----------------- |
| [YOLOv8n](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8n.pt) | 640                   | 37.3                 | 80.4                           | 0.99                                | 3.2                | 8.7               |
| [YOLOv8s](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8s.pt) | 640                   | 44.9                 | 128.4                          | 1.20                                | 11.2               | 28.6              |
| [YOLOv8m](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8m.pt) | 640                   | 50.2                 | 234.7                          | 1.83                                | 25.9               | 78.9              |
| [YOLOv8l](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8l.pt) | 640                   | 52.9                 | 375.2                          | 2.39                                | 43.7               | 165.2             |
| [YOLOv8x](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8x.pt) | 640                   | 53.9                 | 479.1                          | 3.53                                | 68.2               | 257.8             |


## Run
```commandline
streamlit run app.py
```
Then will start the Streamlit server and open your web browser to the default Streamlit page automatically.