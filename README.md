Note: You need to download weights file from the given link. It is recommended to download the whole zip file to run the code easily without issues.
https://drive.google.com/file/d/1rJ7x0X3NHYa065uLa7keBtjFVurXVGK8/view?usp=sharing

# Detecting-custom-objects-in-an-image-video-using-YOLO-V3
YOLO is the state of the art and industry used algorithm for object detection these days. This does the classification/detection by creating grids in the whole image and achieves high accuracy at a very good speed and in real time. We use a pre-trained model which has been trained on the COCO dataset and performs object detection which a very high degree of accuracy. 

Dataset Description:
The dataset used to train the model is COCO dataset. It is a very large dataset for object detection and segmentation. It is the standard dataset to evaluate large scale object detection models. Here, it was trained on 80 classes which is mentioned in the coco.names file in the yolo-coco folder.
Screenshot of coco.names file describing on what objects was yolo trained on.
![image](https://user-images.githubusercontent.com/88571564/178117747-d42d9bfb-5ff9-4d92-a044-87a62922710f.png)

 
Algorithm Description:
YOLO is an abbreviation word for “You look only once”, where this algorithm has shaken most of the developers all around the world in the past 5 years, due to its immense ability to quickly learn and remember any object we have trained or labeled it. There is a unique method to work with Yolo models where we require the images to be labeled firstly using specific tools available online or installing it in your local machine. (Labeling software’s links are provided below). The labeling process might take a long time depending upon on your dataset. The images are labeled according to the specification made by the user, whether we'd like to detect multiple objects in an image are single object, depending on it, the text file is created with following parameters,
+ The class of the objects, starting from 0,1, 2.
+ The coordinates of the bounding box drawn.

Reference
1.	https://machinelearningknowledge.ai/introduction-to-yolov5-object-detection-with-tutorial/
2.	https://pytorch.org/hub/ultralytics_yolov5/
3.	https://github.com/ultralytics/yolov5
To have your own custom object detection, your data needs to be in the following format: 
Sample Label File
The Label file consists of following items.
+ The class of the object
+ Top left coordinate of the bounding box
+ Top right coordinate of the bounding box
+ Bottom left coordinate of the bounding box
+ Bottom right coordinate of the bounding box
 
![image](https://user-images.githubusercontent.com/88571564/178117758-940c28d9-2e2a-4e8a-af46-491167a8d91e.png)

Run command pip install -r requirements.txt or conda install requirements.txt (Requirements.txt is a text file consisting of all the necessary libraries required for executing this python file. If it gives any error while installing libraries, you might need to install them individually.)
 
All the necessary files will get downloaded. To run the code, open anaconda prompt. Go to virtual environment if created or operate from the base itself and run either yolo.py or yolo2.py or yolo_webcam.py as per your requirement.
yolo.py: To run this type python yolo.py --image images/eagle.jpg  #change image as you wish, the image you want to perform detection upon should be in images sub-folder
 ![image](https://user-images.githubusercontent.com/88571564/178117788-9f5b0e13-2d7b-452e-a25b-548f32f55420.png)


 
yolo_webcam.py: To run this type python yolo_webcam.py
 
This will perform real-time object detection
![image](https://user-images.githubusercontent.com/88571564/178117792-813f76ab-0e06-49d0-b08a-3c03a964364c.png)
 
Press “Esc” key to stop the object detection

Issues faced/ Points to note:
1.	Ensure you have all libraries installed.
2.	Give correct paths wherever necessary.
To read more about yolov3, refer to this link https://pjreddie.com/darknet/yolo/
