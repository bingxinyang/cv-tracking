# cv-tracking 

## Introduction 
Our team set out to implement, compare, and contrast traditional computer vision (CV) and deep learning (DL) algorithms for single object tracking, specifically with the aim of helping us casual, yet clueless sports spectators to better understand what is going on during a game by tracking a particular player on the field or court. 

## Datasets 
Two datasets were used to assess the tracking algorithms. The first was the VOT2016 benchmark, which includes 60 sets of image sequences exhibiting a variety of challenging scenarios like occlusion, illumination changes, blurriness, high levels of deformation, and more. Although the VOT2016 dataset uses rotated rectangles, we chose to run our assessments using unrotated rectangles  
VOT16 and OTB50 

<p align="center"><img src ="https://github.com/bigdayangyu/cv-tracking/blob/master/Image_result/kcf.png" width = 60% /></p>

## Run the project
### Prerequisite 
* python 3.5.2
* selective-search
* numpy 
* openCV python 

### KCF trackers 
![](blob/master/Image_result/name-of-giphy.gif)

### GUI

<p align="center"><img src ="https://github.com/bigdayangyu/cv-tracking/blob/master/Image_result/GUI.jpg" width = 60% /></p>

To run the GUI, simply change the path for the video sequence 
```python
    path = {"KCF": './datasets/gui_dataset_kcf/', 
            "MDNet": './datasets/gui_dataset_mdnet/', 
            "SiamFC": './datasets/gui_dataset_siamfc/'}
```
And then run the tracker_gui.py file 
```bash
python /GUI/tracker_gui.py
```
