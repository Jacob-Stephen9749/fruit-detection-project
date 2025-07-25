
# fruit detection

 detects if apples or bananas are ripe rotten or not ripe

multiple images of what ai thinks the fruit is
![val_batch2_labels](https://github.com/user-attachments/assets/d63494c4-94a7-4b14-b290-3520c259eaa8)


## Overview
The AI is first trained to reconize the diffrence between the diffrent fruits and quality of them. after thit the run 2 diffrent commands through YOLOv8 to detct the given fruit and weather it is ripe or not. this is done through either a live feed or a random provided image. 
 

## Installation

Install YOLOv8

```bash
pip install ultralytics
```

Train the model
```bash
yolo task= classify mode=train
```

test the model
```bash
yolo task=classify mode=predict  model=/home/nvidia07/final_project/runs/classify/train4/weights/best.pt source=0
```

use the model to make predictions
```bash
yolo task=classify mode=predict  model=/home/nvidia07/final_project/runs/classify/train4/weights/best.pt source=/home/nvidia07/final_project/runs/classify/predict/test07/final_project/runs/classify/train4/weights/best.pt 
```

