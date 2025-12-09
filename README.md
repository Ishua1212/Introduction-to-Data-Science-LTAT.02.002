# Introduction-to-Data-Science-LTAT.02.002
# Leaf Classification

### Team D5
- Egert Koppel - EK023
- Kaido Kossas - DeadKai
- Sander Miller - Ishua1212

## Goal  
The goal of this project, based on the Kaggle Leaf Classification competition, is to build a
machine learning model that can automatically identify plant species from leaf characteristics
or straight from images. Identifying plant species by hand takes time, requires expertise and
can lead to mistakes. An automated model can speed up the task and help users classify
leaves more consistently.

## Description  
This project implements multiple machine learning approaches to classify leaf images into 99 different species. We explore traditional machine learning models, deep neural networks, convolutional neural networks and ensemble methods to achieve the best classification accuracy.

## What's Included

### Data
- Training data (990 samples with 192 features)
- Test data (594 samples with 192 features)
- Images (1584 leaf images)
- Source: https://www.kaggle.com/competitions/leaf-classification/data

### Trained Models
- Decision Tree model
- Random Forest model (best performing traditional ML model)
- K-Nearest Neighbors model
- Logistic Regression model
- Deep Neural Network (TensorFlow/Keras)
- Convolutional Neural Network (TensorFlow/Keras)
- Support Vector Classifier

### Submissions
- Individual model submissions
- Ensemble submissions (weighted average and max voting)



## Replicating the workflow
- Clone the repository
- Start jupyter notebook
- pip install numpy pandas scipy matplotlib seaborn opencv-python pillow scikit-image scikit-learn joblib tensorflow==2.10.1
- Run the notebook
- (Tensorflow==2.10.1 is needed for using GPU)
 ## Optional / Additional Sections  
- Poster and PDF: See `D5-report.pdf` for detailed project report
- Kaggle Competition: https://www.kaggle.com/competitions/leaf-classification/overview

## Structure
```
├── Data/                  
│   ├── images/              # 1584 leaf images
│   ├── train.csv            # Training data with features
│   ├── test.csv             # Test data with features
│   ├── train_feat.csv       # Training data with extracted features
│   ├── test_feat.csv        # Test data with extracted features
│   └── sample_submission.csv   # Sample submission file
│
├── Models/                 
│   ├── CNN/                 # Convolutional Neural Network
│   ├── SimplerModels/       # Simple models
│   ├── NN/                  # Deep Neural Network
│   ├── svc_leaf_model.pkl   # Support Vector Classifier
│   └── svc_pipeline_with_extracted_features.joblib   # Support Vector Classifier with extracted features
│
├── Notebooks/               
│   ├── Data_inspection.ipynb      # Exploratory data analysis
│   ├── SimplerModels.ipynb        # Simple models (DT, RF, KNN, LR)
│   ├── DeepNeuralNetwork.ipynb    # DNN and SVC with feature extraction
│   ├── CNN.ipynb                  # Convolutional Neural Network
│   └── Ensemble.ipynb             # Ensemble of multiple models
│
└── Submissions/             # Kaggle submission files
```
