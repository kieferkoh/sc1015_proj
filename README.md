# DETECTING FRESH FRUIT

# About
This is a mini project for SC1015 (Data Science and Artificial Intelligence) which implements image recognition models to detect between rotten and fresh fruits

Our motivation for this project stems from commonly seen orange juice machines that are placed around our campus, shopping centres and other prominent locations. We wanted to investigate the feasibility of a image recognition model in vetting the condition of the oranges in the juice machine to make sure it has not become rotten

# Contributors

@ Kiefer - Exploratory Data Analysis & Visualisation, Convolutional Neural Network (CNN) Model, Grad-CAM heatmap     
@ Soham - Data Cleaning & Preparation, Data-driven insights      
@ Marcus - Convolutional Dictionary Learning Model (CDL), KMeans Clustering, Purity Scores      

# Models used
Convolutional Neural Network    
Convolutional Dictionary Learning Model    
KMeans Clustering     
Purity Score      
Grad-CAM      

# Notebooks
1) cdl.ipynb (our implementation)     
2) cnn.ipynb (conventional implementation)     
3) eda.ipynb (exploratory data analysis)    
4) dataclean.ipynb (data cleaning)    

**=====CDL.IPYNB (1)=====**    
This code provides a method for classifying oranges into two categories: fresh and rotten. The classification is performed using a two-layer Convolutional Dictionary Learning (CDL) and clustering-based approach, specifically K-Means clustering.

The main steps of this approach are:

Load the orange images dataset and preprocess the images.
Perform Convolutional Dictionary Learning (CDL) in a two-layer structure.
Estimate the sparse representation (coefficient maps) for the training data using the learned dictionaries.
Apply clustering on the learned representations to perform classification.
Evaluate the performance using purity and Rand Index metrics.
Usage
To run the code, you need to have the dataset of orange images stored in a "data" folder, with two subfolders: "freshoranges" and "rottenoranges". The dataset should contain labeled images of fresh and rotten oranges.

The main method to run the classification process is the make_option() function, which sets the options for the CDL layers and the number of training and testing samples.

After running the code, you will get the performance metrics for the K-Means clustering using Euclidean and Mahalanobis distances.

**Dependencies**

The code requires the following libraries:  

numpy
cv2
os
sporco
sklearn
SF_KMeans
skimage
torchvision
Make sure to install the required libraries before running the code.

=====CNN.IPYNB (2)=====    
This notebook instantiates a Convolutional Neural Network model, with 3 filter layers    
The data is split into 70% train data, 20% validation data and 10% test data to be sourced into the model    
This model achieved a 50% accurate prediction rate between fresh and rotten oranges.     

**Dependencies**

The code requires the following libraries:  
os
tensorflow
cv2
numpy
pandas
matplotlib

=====EDA.IPYNB (3)=====     
This notebook aims to perform Exploratory Data Analysis (EDA) for our dataset, gathering data for pre-processing to be used in our model    
- Analysing dataset distribution    
- Visualisation of dataset    
- Inspecting dataset properties    
**Dependencies**

The code requires the following libraries:  

os
matplotlib
random  

=====DATACLEAN.IPYNB (4)=====     
This notebook removes duplicates and outliers from the dataset using hash functions and by comparing the frequency property of the images.  
**Dependencies**

The code requires the following libraries:  
imagehash tensorflow  

# Limitations and Improvements
Currently our model can only predict the freshness of a fruit based solely on its looks from the outside, hence some oranges which are rotten on the inside but look fine on the outside may be misclassified.
To overcome this limitation in a future model, an additional dataset of images of oranges once they've been cut can be included can be used for training, and then the oranges could be checked for freshness twice, once before being cut and once after. By having an additional layer of checking, the model accuracy will be near perfect.

# References
Please find the references used in the last two slides of the presentation file attached.
