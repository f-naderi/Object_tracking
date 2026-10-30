```markdown
# Object Tracking and Optical Flow Analysis

A computer vision project for object detection, tracking, and motion analysis in dashcam videos using YOLO, and Optical Flow (RAFT & OpenCV).

## Features

- Object detection using YOLO (Ultralytics)
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

- YOLO: Ultralytics 
- Teed, Z., & Deng, J. (2020, August). Raft: Recurrent all-pairs field transforms for optical flow. In European conference on computer vision (pp. 402-419). Cham: Springer International Publishing.
- Lucas, B. D., & Kanade, T. (1981, August). An iterative image registration technique with an application to stereo vision. In IJCAI'81: 7th international joint conference on Artificial intelligence (Vol. 2, pp. 674-679).
- Farnebäck, G. (2003, June). Two-frame motion estimation based on polynomial expansion. In Scandinavian conference on Image analysis (pp. 363-370). Berlin, Heidelberg: Springer Berlin Heidelberg.
- Dashcam Input Video (YouTube). [Video Source](https://youtu.be/JHf2u7TqUEY?si=fth2Sa9uYWDMnqDC)

```
