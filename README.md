# Comparative-Analysis-of-YOLO-Models
Comparative Analysis of YOLO Models for Real-Time Detection Trained on Indian Driving Dataset (IDD)

Real-time object detection is crucial for modern automation. 
While current state-of-the-art models perform well on structured Western roads, deploying these systems in an unstructured environment such as Indian streets with high traffic density and localized vehicle types presents a unique challenge. 
Furthermore, to run these heavy neural networks, expensive, cloud computing hardware is required. 
This project evaluates the feasibility of deploying a localizable, real-time object detection pipeline on a standard, consumer-grade computer. 

To address this, three sizes of the single-stage detector, YOLOv8 (Small, Large, and Extra-Large), were trained and evaluated using the Indian Driving Dataset (IDD). 
The objective was to identify the trade-offs between model size. 
This was measured in accuracy (mAP), and processing speed (latency in milliseconds) when running on local hardware.

The metrics were collected inside Jupyter Notebook using YOLOv8's native validation engine, and the results were plotted using Matplotlib. 
A custom inference pipeline was built using OpenCV to print the model’s inference speed directly on top of the image. 
It was run locally on an NVIDIA RTX 3070 Laptop GPU with 8 GB of VRAM. 
