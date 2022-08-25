# Crosswalk-Detection with YOLOv3 Model

### Description  
This project is implemented based on a Computer Vision model. We used a pretrained model YOLOv3 and transfer learning to detect crosswalks in any street.   

### Repo structure  

* `1_Image_Annotation`: Scripts and instructions on annotating images
* `2_Training`: Scripts and instructions on training your YOLOv3 model
* `3_Inference` Scripts and instructions on testing your trained YOLO model on new images and videos
* `Data`: Input Data, Output Data, Model Weights and Results
* `Utils`: Utility scripts used by main scripts  

![Structure](images/structure)

### Installation
#### step 1/ Clone the repo
`git clone 'https://github.com/YuriHFlowers/MyOwnModelYolo'`

#### step 2/ Create a Virtual Environment or you can download in Google Colab too.

#### step 3/ Install Required Packages
Use `pip install requirements.txt` for installation.

### Usage  

Follow these steps to run the program for your custom dataset:

1. First, prepare the dataset:
You need to feed your model with training examples to have a good detector. For this task you can use Microsoft's Visual Object Tagging Tools `VoTT` to label the images manually.   
Follow the instructions in `1_Image Annotation\README.md` for downloading VoTT in Mac, Windows or Linux. Then you can create your own annotations for your training images. 

2. Train your own Yolo model:
First, you need to convert the `Pre-trained Weights`. You can follow the specific instructions in the `2_Training\README.md`.
Then, you can train the model running `python Train_YOLO.py`.

3. Detect crosswalk in your testing images:
Run the script `python Detector.py`. The results will be stored in the `TrainYourOwnYOLO/Data/Source_Images/Test_Image_Detection_Results` folder.  
   
### Result View
![crosswalk](images/crosswalk.png)

### Colaborators
Yuri Hernández Flores  
Rana Abuthaher  
Chaitali Sonawane  

These scripts are taken from https://github.com/AntonMu/TrainYourOwnYOLO
  
### Future improvements
Train the model with more images.  
During the trainning we noticed that the most of the images were taken from the right side, so for improving the training we propose to have another dataset with pictures taken from the other side.  
Make the hyperparameter optimization for tuning the model.  


