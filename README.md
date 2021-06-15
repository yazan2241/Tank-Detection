# Tank-Detection
Tank Detection Weights

![altay_l3](https://user-images.githubusercontent.com/34937698/122085567-d7106680-cdd0-11eb-83b4-3c4c0756df13.jpg)


# Goal of this project

I searched the internet previosly for a Tank model Detector but i could not fond any model or pretrained weights that do this
so i trained Yolo model for detection a Tank in a picture

# Built With 🛠

  the mode have been trained on 2000 images from Open Images Dataset
  https://storage.googleapis.com/openimages/web/index.html

  used this Repository for Converting the Annotation to Yolo V3 format
  https://github.com/theAIGuysCode/OIDv4_ToolKit

  Yolo V3 model https://pjreddie.com/darknet/yolo/
 
  
 # Usage
  
  make sure you downloaded open cv befor start
  
  download the pretrained weights feom this link
  https://drive.google.com/file/d/1mjmSb5OG2ZmtEn7opmvoip3GuI9B4390/view?usp=sharing
  
  - clone this repository
  
  - in the yolo_object_detection.py file  you have to change the weights file path to where you download it
   (8 line)   net = cv2.dnn.readNet("yolov3_training_last.weights", "yolov3_testing.cfg")         #put full path for weights file
   (14 line) images_path = glob.glob(r"E:\python\images\*.jpg")                                   # put full path for test images directory
   
  - Prepare test images from Kaggle dataset or from google or from where ever you want
   
  - Run the code <python yolo_object_detection.py>
  
  
  
  # Note
  this project trainedonly to detect Tanks .. so if the picture conatin Cars it might detect it too since it looks similar (in general) to the Tanks
  check updates for the repository .. i am working on updating the model
  
  # Test
  
  ![1](https://user-images.githubusercontent.com/34937698/122087998-59018f00-cdd3-11eb-97f5-539b0e891d88.png)
![3](https://user-images.githubusercontent.com/34937698/122088125-76cef400-cdd3-11eb-97a8-980fbcc21289.png)
![4](https://user-images.githubusercontent.com/34937698/122088311-98c87680-cdd3-11eb-9c07-7e22de268c98.png)
![2](https://user-images.githubusercontent.com/34937698/122088328-9cf49400-cdd3-11eb-98f9-522a7e045764.png)


  
  
  
