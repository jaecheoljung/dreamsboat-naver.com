# Action Localization

Step 1. Action recognition
 - 
 
Step 2. Localization
 - To do.


## Training

[APS dataset](https://drive.google.com/file/d/1VFM1J2yem5L3m6Zabefv6Qveeh4DXnUj/view?usp=sharing)

Unzip dataset in root directory.

'
python split_video.py aps_original aps_cut
python train.py
'

will generate folder name 'data' and put all video clips there.

if you want to test with unseen dataset,

'
python test.py
'