# Action Localization

Step 1. Action recognition (modified. original code source: https://github.com/jfzhang95/pytorch-video-recognition)
 - Accuracy
 
 
   Train accuracy over 99%
 
 
   Top validation accuracy over 97%
 
 
Step 2. Localization
 - Using YOLO v3 (modified. original code source: https://github.com/ayooshkathuria/pytorch-yolo-v3)

<p align="center"><img src="yolov3/video_output/demo.gif" align="center"></p>

## Classification Training

Download [APS dataset](https://drive.google.com/file/d/1VFM1J2yem5L3m6Zabefv6Qveeh4DXnUj/view?usp=sharing)

Unzip dataset in root directory.

`python split_video.py aps_original aps_cut` 
will make a new folder named 'aps_cut' and put all split videos there.

`python train.py`
will make a new folder named 'data' and start training.

Training Results are like below.

<p align="center"><img src="C3D.JPG" align="center"></p>

validation accuracy

<p align="center"><img src="validation_acc.JPG" align="center"></p>

validation loss

<p align="center"><img src="validation_loss.JPG" align="center"></p>


### YOLO v3
Go to yolov3 directory.

Download pre-trained weight [here](https://pjreddie.com/media/files/yolov3.weights)

`python video.py --video video_input/aps.avi video_output/`
