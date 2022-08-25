# Crosswalk-detection


### Description  
This project is implemented based on deep learning model. Using a pretrained model YOLOv3 to detect the crosswalk in any street.   

### Repo structure  
* 1_Image_Annotation: Scripts and instructions on annotating images
* 2_Training: Scripts and instructions on training your YOLOv3 model
* 3_Inference: Scripts and instructions on testing your trained YOLO model on new images and videos
* Data: Input Data, Output Data, Model Weights and Results
* Utils: Utility scripts used by main scripts  

### Pipeline Review
![webapp](Yolo_model_structure)

### Installation
#### step 1/ clone the repo
`git clone 'https://github.com/YuriHFlowers/MyownYolo'`

#### step 2/ Create Virtual Environment

#### step 3/ Install Required Packages
Use `pip install requirements.txt` for installation.

### Usage  
Follow these steps to run the program for custom dataset:

1. Start with preparing the dataset
To have a good detector, we need to feed our model some good training examples. Using Microsoft's Visual Object Tagging Tools `VoTT` to label the images manually. follow the instructions in `1_Image Annotation\README.md` for downloading this tool, how to use it, saving the new dataset in `Training_Images`, and creating the annotation file.

2. follow the instructions in `2_Training\README.md` for downloading and converting the
`Pre-trained Weights`.

3. Train the model using `python Train_YOLO.py`.

4. To detect object run the script `python Detector.py`. The output will be saved in 
   `TrainYourOwnYOLO/Data/Source_Images/Test_Image_Detection_Results`

 The original source for the pretraind YOLO model 

### Result View
![webapp](static/clustering_result.png)

### Future improvements


