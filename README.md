AppliedML - Assignment 1

## 1&2 steps: Photos and their annotation on roboflow

I took photos of my cup and my e-cigaret. Annotated them using roboflow. Examples are:

1.  <img src="https://drive.google.com/uc?export=view&id=10gQTQaDbGQA7V9NEB8CQwj7LDtyYnx-E" width="300" align="center" hspace="40px">

2.  <img src="https://drive.google.com/uc?export=view&id=1HDRQgBNQt31_sYQr_XZKL7kv7kPAvpwT" width="300" align="center" hspace="40px">

## 3 step: Faster-RCNN training results

Results are as follows: mAP: 80% for class cigaret
My second class wasn't detected. My suspicion is that I misconfigured the Faster-RCNN and didn't specify number of classes.
But re-run would took a lot of time as my number of iterations is 2000. Training took over hour and half

## 4 step: YOLO-8n training results

For YOLO, there was no problems with detecting both of my objects.
mAP for cigaret: 0.78
    for cup: 0.66

Such results could be explained by size of the model. 10% difference between 2 classes could be explained by dataset and quality of photos taken

With small dataset size i used low amount of epoch not to overfit nanomodel


Faster-RCNN Notebook: https://colab.research.google.com/drive/1WyyhFEPYjlUcZhyaFRhLb3W7kuEQ1ZHv?usp=share_link
YOLO Notebook: https://colab.research.google.com/drive/1rlvSo_uTxeKz2oHmW8uvrpYLF2rV6G8q?usp=share_link
