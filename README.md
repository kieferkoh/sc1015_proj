# DETECTING FRESH FRUIT

# About
This is a mini project for SC1015 (Data Science and Artificial Intelligence) which implements image recognition models to detect between fake and fresh fruits

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

=====CDL.IPYNB (1)=====    
     
     
=====CNN.IPYNB (2)=====    
This notebook instantiates a Convolutional Neural Network model, with 3 filter layers    
The data is split into 70% train data, 20 validation data and 10% test data to be sourced into the model    
This model achieved a 65% accurate prediction rate between fresh and rotten oranges.     
      
=====EDA.IPYNB (3)=====     
This notebook aims to perform Exploratory Data Analysis (EDA) for our dataset, gathering data for pre-processing to be used in our model    
- Analysing dataset distribution    
- Visualisation of dataset    
- Inspecting dataset properties    
      
=====DATACLEAN.IPYNB (4)=====     
