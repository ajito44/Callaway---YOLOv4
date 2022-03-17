# Callaway---YOLOv4

# This repository alone will not run YOLOv4. To download and run YOLOv4 please pull: https://github.com/AlexeyAB/darknet or read through https://pjreddie.com/darknet/yolo/ 

- Use **Visual Studio Code** to run the program: https://code.visualstudio.com/

## This project is for the Callaway Golf Measurement System.

- For reference to Fall21': https://github.com/anwarhsu/golf-detection
- For training on YOLOv4: https://github.com/AlexeyAB/darknet#how-to-train-to-detect-your-custom-objects or https://github.com/AlexeyAB/darknet
- For annotating images: https://github.com/tzutalin/labelImg

## This repository contains all the necessary files to run YOLOv4 with our custom requirements:
 - Configuration File (good for two objects): **yolov4.cfg**
 - Weight file (previous group): https://drive.google.com/file/d/1B519piHVWGLYfzDS1By_8OI9UzCFqtvy/view?usp=sharing
 - Weight file (YOLO): https://newreleases.io/project/github/AlexeyAB/darknet/release/darknet_yolo_v4_pre
 - Images for training: https://drive.google.com/drive/folders/1-AhevnDRzTTQD7fhwJYCs97crFWCRsGw?usp=sharing
 - Files for training: **obj.data, train.txt, obj.names**
 
## If trying to run https://github.com/anwarhsu/golf-detection on a MacOS, the terminal commands are as follows: 
- Steps 1 and 2 are the same

- Step 3: 
```
pip install virtualenv
python3 -m venv .venv
source .venv/bin/activate
```
- Step 4 is the same

## To run YOLOv4 on a MAC:

### Detect
```
 ./darknet detect cfg/yolov4.cfg [WEIGHT FILE NAME] [IMAGE NAME]
 ```
 *NOTE: cfg/yolov4.cfg is the configuration file, use the necessary configuration file needed
 
 ### Train
 
 ```
 ./darknet detector train data/obj.data yolo-obj.cfg yolov4.conv.137
 ```
 *NOTE: this is just an example
 
 ### Basically, for MacOS use
  ```
  ./darknet
   ```
   for every command, instead of
    ```
    darknet.exe
     ```
    
 
 
