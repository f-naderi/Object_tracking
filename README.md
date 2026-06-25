```markdown
# Object Tracking & Optical Flow Analysis

A computer vision project for object detection, tracking, and motion analysis in dashcam videos using YOLO, and Optical Flow (RAFT & OpenCV).

## Features

- Real-time object detection using YOLO (Ultralytics)
- Multi-object tracking (YOLO tracking)
- RAFT optical flow (PyTorch)
- Classical optical flow (Farneback method)
- Motion analysis over time (mean flow magnitude)
- Video visualization and export (MP4 output)

## Project Structure

Object_tracking/
├── runs                          # YOLO outputs and results
├── Farneback_output.mp4          # Farneback optical flow output video
├── raft_output.mp4               # RAFT optical flow output video
├── video.mp4                     # Input dashcam video
├── Object_tracking.ipynb         # Main Jupyter notebook
└── requirements.txt              # Python dependencies

## Installation

```bash
git clone https://github.com/f-naderi/Object_tracking.git
cd Object_tracking
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
```


## Results

Object Detection Overall Performance

- mAP@50: **0.863**
- mAP@50-95: **0.644**
- Precision: **0.864**
- Recall: **0.790**

Observation

- RAFT produced **smoother and more physically consistent motion fields**
- OpenCV Farneback showed **more noise and artifacts**


Motion Analysis

- Clear spike was observed during scene transition


## Requirements

* Python 3.10+
* PyTorch
* Ultralytics YOLO
* OpenCV
* Matplotlib
* NumPy
* Jupyter Notebook


## References

- YOLO: Ultralytics (2023)
- RAFT: Teed & Deng (2020)
- Optical Flow: Lucas-Kanade (1981)
- Farneback Method: Gunnar Farneback (2003)
- Dashcam Input Video (YouTube). [Video Source](https://youtu.be/JHf2u7TqUEY?si=fth2Sa9uYWDMnqDC)

```
