# Traffic Sign Recognition Using Deep Learning

## Project Overview
This project implements a deep learning model to accurately recognize and classify traffic signs from images. Using Convolutional Neural Networks (CNNs), the model aims to provide reliable traffic sign recognition under diverse real-world conditions, such as different lighting, occlusions, and weather. This project can be applied in the development of autonomous vehicles and advanced driver-assistance systems (ADAS).

## Table of Contents
- [Problem Definition](#problem-definition)
- [Objective](#objective)
- [Dataset](#dataset)
- [Methodology](#methodology)
- [Results](#results)
- [Installation](#installation)

## Problem Definition
Traffic signs are critical for road safety, especially for autonomous driving and driver assistance technologies. Recognizing these signs accurately in real-time is challenging due to variations in lighting, angles, and visibility conditions. This project aims to improve traffic sign recognition accuracy and robustness using a CNN model trained on a diverse dataset.

## Objective
1. Achieve high classification accuracy across various types of traffic signs.
2. Build a model capable of generalizing across different real-world conditions.
3. Develop a solution suitable for real-time applications in autonomous vehicles.

## Dataset
The model is trained on the [German Traffic Sign Recognition Benchmark (GTSRB)](https://benchmark.ini.rub.de/) dataset, which includes over 50,000 images of traffic signs belonging to 43 different classes.

## Methodology
1. **Data Preprocessing**: The images are resized and normalized. Data augmentation techniques like rotation, scaling, and shifting are applied to increase model robustness.
2. **Model Architecture**: A CNN is designed with multiple convolutional and pooling layers to extract features, followed by fully connected layers for classification.
3. **Training and Evaluation**: The model is trained with cross-entropy loss and optimized with the Adam optimizer. Performance metrics such as accuracy and F1-score are used for evaluation.

### Model Architecture
The CNN model consists of:
- Convolutional layers with ReLU activation
- Max-pooling layers
- Fully connected layers
- Dropout layers to prevent overfitting

## Results
The CNN model achieved an accuracy of **[your model’s accuracy]** on the test set. The model was able to classify traffic signs with high accuracy across various conditions, demonstrating potential for real-world applications.

## Installation
To run the project locally, follow these steps:

1. **Clone the repository**:
   ```bash
   git clone https://github.com/your-username/traffic-sign-recognition.git
   cd traffic-sign-recognition
2. **Create a Virtual Environment (Optional but Recommended)**:  
   Setting up a virtual environment helps to manage dependencies:
   ```bash
   python -m venv venv
  - **Activate the Virtual Environment**:
    - On **Windows**:
      ```bash
      venv\Scripts\activate
      ```
    - On **macOS/Linux**:
      ```bash
      source venv/bin/activate
      ```
3. **Install Dependencies**:  
   Install the required Python packages using the `requirements.txt` file by running:
   ```bash
   pip install -r requirements.txt

4. **Download and Prepare the Dataset**:
   -Download the German Traffic Sign Recognition Benchmark (GTSRB) dataset.
   -Unzip the dataset and place it in a folder named data/ within the project directory.
