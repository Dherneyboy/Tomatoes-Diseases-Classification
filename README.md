# Tomato Diseases Classification & Deployment using Convolutional Neural Network and FastAPI
This repository contains a project on classification of tomato diseases using Convolutional Neural Network and deployed using FastApi
## Overview of Leaf Disease
Tomato plants are susceptible to a variety of leaf diseases, primarily caused by fungi, bacteria, and environmental conditions. These diseases can significantly impact the health and yield of tomato crops. Some of the most common tomato leaf diseases include:
1.	Early Blight: Caused by the fungus Alternaria solani, early blight manifests as dark spots with concentric rings on the lower leaves. properly.
2.	Late Blight: This disease, caused by the water mold Phytophthora infestans, is notorious for its rapid spread and devastating impact. It appears as water-soaked lesions on leaves, which quickly turn brown and can destroy entire plants.
3.	Septoria Leaf Spot: Characterized by small, circular spots with dark borders and gray centers, this fungal disease (Septoria lycopersici) primarily affects the lower leaves, leading to premature leaf drops.
4.	Bacterial Spot: This bacterial disease (Pseudomonas syringae pv. tomato) causes small, dark spots on leaves and fruit. It is often exacerbated by cool, wet conditions.
Effective management of these diseases involves a combination of cultural practices, such as crop rotation, proper spacing, and sanitation, as well as the use of resistant varieties and appropriate fungicides or bactericides

This project aims to classify tomato leaf images into different disease categories using a Convolutional Neural Network (CNN). We trained the model on the PlantVillage dataset from Kaggle, which contains labeled images of healthy tomato leaves and leaves affected by various diseases. The model was deployed using Fast Api.

## Project Structure
- Data/: Contains the dataset (you can download it from the Kaggle link above).
- notebooks/: Jupyter notebooks for data exploration, model training, and evaluation.
- src/: app.py: FastAPI app for serving predictions.
- model/: Saved trained model weights.
- requirements.txt: List of Python dependencies.

## Getting Started
1.	Data Preparation:
- Download the PlantVillage dataset and place it in the data/ directory. 
- Preprocess the images (resize, normalize, etc.).
2.	Model Training:
- Run train.py to train your CNN model.
- Experiment with hyperparameters, architecture, and data augmentation.
3.	Model Deployment:
- Use FastAPI to create an API for serving predictions.
- Run uvicorn app: app --reload to start the server.
4.	Make Predictions:
- Send POST requests to http://localhost:8000/predict with an image file.
- Receive JSON responses with predicted classes and probabilities.

## Tools Used
- Programming Language: Python
- Libraries: Pandas, Numpy, Matplotlib, Sklearn, seaborn, TensorFlow, Keras, FastAPI.

## Model Evaluation and Result
A Convolutional Neural Network was used to classify Tomato diseases. The data below shows the graphs of the Training and Validation Accuracy & Training and Validation Loss.

![image](https://github.com/user-attachments/assets/1ee9eb59-b2fb-48b4-9dba-b7967c743cb2) ![image](https://github.com/user-attachments/assets/4e917ec9-55b1-4e6c-b3fc-4ad52c647c17)


  
## Acknowledgments
- Codebasics: https://www.youtube.com/watch?v=Mubj_fqiAv8&list=PLeo1K3hjS3uu7CxAacxVndI4bE_o3BDtO
- The PlantVillage dataset:  https://www.kaggle.com/datasets/arjuntejaswi/plant-village
- FastAPI documentation: FastAPI






