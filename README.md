#**Road sign recognition and visual operation based on yolov5**

##**Abstract**

  Aiming at addressing the distinct problem in road sign recognition, this paper utilizes the TT100K dataset as training data, and implement the YOLOv5 network model to detect and recognize road signs. In general, road sign recognition systems are usually employed when cars are moving at high speeds. As a result, high accuracy and real-time performance are required when handling road signs. When accessing the conventional YOLOv5 network, the model has a long duration and the system responds sluggishly due to the great capacity of this model. For the purpose of tackling this problem, this paper adds a CBAM (Channel Block Attention Module) attention mechanism, and combines the MobileNetv2 lightweight network to optimize the YOLOv5s network model. The improved YOLOv5s_M2C network can recognize road signs faster in a higher precision. Our method not only enhances the recognition accuracy, but also speeds up the recognition rate.
***
##**Package Requirement**

  To run this code, some packages are needed as following,You can install these packages using requirements.txt.
```
matplotlib>=3.2.2
numpy>=1.18.5
opencv-python>=4.1.2
Pillow
PyYAML>=5.3.1
scipy>=1.4.1
torch>=1.7.0
torchvision>=0.8.1
tqdm>=4.41.0
tensorboard>=2.4.1
seaborn>=0.11.0
pandas
thop  # FLOPS computation
pycocotools>=2.0  # COCO mAP
```
***
##**Dataset**

  **TT100K**
  
  It is a road sign dataset that is currently open in China. It is a large-scale and high-quality road sign dataset. This paper analyzes and sorts out the TT100K dataset, combines the TT100K dataset with the TSRD dataset, uses reptiles to supplement the dataset, and uses data amplification strategies to solve some data shortages.
  
  **If you want to use your own dataset**
  
  You can put your dataset in./VOCdevkit, and the dataset should be labeled in VOC format.
***
##**Run Code**

  1.Download the project.
  
  2.Follow the comments in code to do something, such as change the path and parameters, move pretrained .
  
  3.Run train.py to train the model you downloaded from the official website of yolov5.
  
  4.Run test.py to test your training model.
  
  5.The results of the training will be in the./runs folder
***
##**PyQt Visual interface**

  Use PyQt5 to add a visual detection interface for YoloV5, and realize simple interface jump, as follows:
  
  **characteristic**:
  
  1.Separation of UI and logic code
  
  2.Support self selected model
  
  3.At the same time, output the detection results and relevant information
  
  4.Support image, video and camera detection
 
  5.Support video pause and continue detection
  
  6.The ui folder stores the py file and the original of the ui for easy use and change
  
  7.ui_ Img stores image files used by the ui
  
  8.A user account tool id is added to utils_ utils.py
  
  9.detect_ Logical.py is the logic code of the detection interface
  
  10.main_ Logic. py is the logic code of the main interface
  
  11.Userinfo.csv stores user account ID information
***

##**Thanks**

  Thanks to all those who participated in this article, and all those who read this article and visited Github project.

