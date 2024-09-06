# AI-UrbanFarming

This project focuses on using AI to detect diseases in tomato plants by analyzing images of tomato leaves. Leveraging CNN and YOLO models, the goal is to enhance urban farming practices by identifying plant diseases early through AI-based image classification.

## Table of Contents
- [Introduction](#introduction)
- [Features](#features)
- [Dataset](#dataset)
- [Model Results](#model-results)

## Introduction
Urban farming is becoming increasingly important as cities aim to produce food locally. One of the challenges is maintaining the health of crops by identifying and treating plant diseases promptly. This project utilizes AI models to detect various diseases in tomato plants by analyzing images of their leaves. By employing advanced deep learning techniques like Convolutional Neural Networks (CNN) and YOLO (You Only Look Once), the system can classify and identify tomato plant diseases with high accuracy, enabling farmers to take timely action.

## Features
- **Disease Detection Models**: Utilizes CNN and YOLO for image-based disease classification specific to tomato plants.
- **Comprehensive Dataset**: Uses a dataset of tomato leaf images with various diseases and healthy leaves.
- **Efficient Image Classification**: Classifies images into multiple disease categories to help identify specific issues affecting tomato plants.
- **Real-Time Analysis**: Potential for integration with real-time monitoring systems in urban farms.

## Dataset
The project uses a dataset of tomato leaf images categorized into the following classes:

- **Tomato_Bacterial_spot**
- **Tomato_Early_blight**
- **Tomato_Late_blight**
- **Tomato_Leaf_Mold**
- **Tomato_Septoria_leaf_spot**
- **Tomato_Spider_mites_Two_spotted_spider_mite**
- **Tomato_Target_Spot**
- **Tomato_Tomato_YellowLeaf_Curl_Virus**
- **Tomato_Tomato_mosaic_virus**
- **Tomato_healthy**

The dataset is split into training, validation, and test sets. Each image is labeled accordingly to facilitate supervised learning.

## Models Evaluated
The following models were evaluated for object classification to identify the plant's growth and health:

- **Custom CNN Model**
- **Xception Model**
- **ResNet50V2 Model**
- **DenseNet121 Model**
- **EfficientNetV2B3 Model**
- **VGG16**
- **MobileNetV2**
- **InceptionV3**
- **InceptionResNetV2**
- **NASNetMobile**

## Model Results

### 1. **EfficientNetV2B3**
EfficientNetV2B3 is ranked first because it delivers the best performance across all key metrics, especially the F1 score and recall. This model is highly effective at both detecting true positives (diseased plants) and minimizing false positives. Its high recall ensures that almost all instances of plant disease are detected, which is crucial for preventing the spread of disease in agriculture. The minimal difference between precision and recall also indicates a well-balanced model.

### 2. **Custom CNN**
The Custom CNN ranks second due to its strong balance between recall and precision, with a high F1 score. This model is specifically designed to detect plant diseases, making it a robust option for this application. Although it does not outperform EfficientNetV2B3, its high recall makes it reliable for detecting most diseased plants, ensuring minimal false negatives.

### 3. **DenseNet121**
DenseNet121 is closely ranked to the Custom CNN, showing strong performance with an F1 score and recall that are nearly identical. This model’s architecture, which efficiently passes information across layers, helps in accurately detecting plant diseases. Its slightly lower F1 score compared to the Custom CNN places it in third, but it still offers excellent reliability in disease detection.

### 4. **MobileNetV2**
MobileNetV2 offers a good trade-off between performance and computational efficiency, making it suitable for mobile or edge devices used in field conditions. Its F1 score and recall are slightly lower than DenseNet121, but it still performs well in detecting plant diseases. The model is ranked fourth because, while effective, it is outperformed by more complex models in terms of precision and recall.

### 5. **ResNet50V2**
ResNet50V2 is a strong model with an F1 score and recall that make it a reliable choice for plant disease detection. Its architecture, which includes skip connections to prevent the vanishing gradient problem, contributes to its robustness. However, it is ranked fifth because other models offer better performance in terms of F1 score and recall, which are crucial for this application.
