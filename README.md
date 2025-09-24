# Brain_tumor_detector
## Intentions:
### Purpose of this model is to live detect Brain Tumor which affects approx. 90,000 people in US alone. With help of Brain_Tumor_detector, anyone can access the techonology to detect the tumor, further determining which type of tumor is in affect helping professionals predicting the tumor with highest accuracy.
## Procedure: 
### Data Handling and Preparation
#### 1. Loading the required datasets is essential. Making a seperate cell for the dedicated purpose would be convinient. 
#### 2. Next step would be loading the required datasets. This task have been achieved with the help of kagle datasets. Here is the link to the dataset: https://www.kaggle.com/datasets/preetviradiya/brian-tumor-dataset.
#### 3. Save all images path to two subdirectories 'yes' or 'no'. Before visualisation process make sure to label these 'yes' and 'no' folder to '1' and '0'. 
#### 4. Using matplotlib and cv2, you can check and visualise the dataset organised in the previous step.
#### 5. Dataset spliting
#### 6. Transforming the data to the consistent format of 244 x 244 pixels. mean=[0.485, 0.456, 0.406], std=[0.229, 0.224, 0.225] are the standard specific mean and standard deviation for imageNet model. 
#### 7. Create custom class to inherit from the dataset and provide the required values like number of images and its path to the working model. 
#### 8. Don't forget to create DataLoaders, it iterates through the dataset and seperate them into baches for the model to train on them easily. 

### Model Artitechture and Modeling
#### 1. Loading pre trained model like MobileNetV2, most powerful model in torchvision for general classification. 
#### 2. Freezing the layers helps not to update the pretrained model wieghts and treating it as a fixed feature extractor. 
#### 3. Updating the classifier is necessary cause original model has final layer designed to output 1000 scores. 

### Model Training and Classification
