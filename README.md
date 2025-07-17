# Car-Damage-Detection


I've created a program that addresses your car damage assessment task using the dataset with the six classes (F_Normal, F_Crushed, F_Breakage, R_Normal, R_Crushed, R_Breakage).


## What is included in this repository?
- A README file
- Jupyter Notebook consisting of the entire code
- Google drive link for train and test sets
- A PowerPoint Presentation

## How to Use
Download the jupyter notebook and the dataset from the given Google Drive link. Set the paths for train and test sets. Modify these two lines in the first cell of notebook.ipynb if you intend to train and run the model on your machine.  
```TRAIN_DIR = "D:/Sem 6/ICV/ICV_Project/dataset/train" ```  
```TEST_DIR = "D:/Sem 6/ICV/ICV_Project/dataset/test"```  

## Prerequisites
To run this program, you'll need:

Python 3.7+ installed  
The following packages:  
TensorFlow 2.x  
OpenCV (cv2)  
NumPy  
Matplotlib   
scikit-learn  
seaborn  

Install these packages using pip:  
```pip install tensorflow opencv-python numpy matplotlib scikit-learn seaborn```

## Program Features
This program includes:

### Image Preprocessing:

Histogram equalization for light adjustments
Image resizing to standard dimensions (224x224)
Color space conversion
Normalization


### Edge Detection and Contour Analysis:

Canny edge detection to highlight damages
Contour visualization to identify structural damage


### Model Architecture:

Transfer learning with MobileNetV2 (faster than VGG for your deadline constraints)
Custom classification head with dropout for regularization
Batch normalization for more stable training


### Advanced Visualizations:

Grad-CAM to visualize which regions of the car influenced the classification
Feature map visualization to understand what the model "sees"
Confusion matrix to evaluate model performance across classes

## How It Works

Image Processing: The program standardizes all images, corrects for lighting variations, and extracts key visual features.

Front/Rear Classification: The CNN architecture naturally learns to distinguish front (F_) vs rear (R_) cars through the training process.

Damage Detection: The model identifies normal vs damaged cars (Crushed, Breakage) by learning the unique visual patterns associated with each damage type.

Visualization: The program provides extensive visualizations to help understand what features the model is using to make its decisions.




  
