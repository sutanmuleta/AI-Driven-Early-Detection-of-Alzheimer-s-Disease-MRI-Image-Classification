# AI-Driven-Early-Detection-of-Alzheimer-s-Disease-MRI-Image-Classification


## Overview

This repository presents an AI-driven approach for the early detection of Alzheimer's disease by classifying brain MRI images. Leveraging the power of deep learning, specifically a fine-tuned ResNet18 model, this project aims to enhance the accuracy and timeliness of Alzheimer's diagnosis, providing critical support for early intervention and better patient outcomes.

## Problem Statement

Alzheimer’s disease is a critical global health issue, with early diagnosis being essential for effective treatment. Traditional diagnostic methods, which rely on clinical evaluations and cognitive tests, often result in late detection, limiting treatment options. As the population ages, the need for more accurate and timely diagnosis has become increasingly urgent.

### Key Challenge:
- How can a machine learning model be developed to accurately classify the stages of Alzheimer’s disease using brain MRI images, enabling earlier diagnosis and better treatment outcomes?

## Project Significance

Early detection of Alzheimer’s disease can significantly impact patient outcomes by enabling timely interventions that can slow disease progression, preserve cognitive function, and improve the quality of life for millions of people worldwide. This project addresses this critical need by developing a model that can identify subtle patterns in MRI images, often missed by human eyes.

## Model Development

### Model Architecture

- **Base Model**: ResNet18, a well-established convolutional neural network (CNN) known for its effectiveness in image classification tasks.
- **Modifications**: 
  - Replaced the final fully connected layer to output predictions for four classes: Non-Demented, Very Mild Demented, Mild Demented, Moderate Demented.
  - Integrated a dropout layer with a 50% rate to prevent overfitting, enhancing model robustness.

### Data Preprocessing

- **Data Augmentation**: Applied techniques such as rotation, flipping, and color jitter to enhance the model's ability to generalize to new, unseen images.
- **Normalization**: Standardized MRI images to ensure consistent input data, improving model performance.

### Training Strategy

- **Optimizer**: Employed the Adam optimizer with a reduced learning rate of 0.0005 to achieve better convergence.
- **Epochs**: Trained the model for 10 epochs, balancing thorough learning with computational efficiency.

## Evaluation and Results

The model was assessed on a separate test set, achieving a foundational accuracy of 58.64%. While this indicates a need for further refinement, it also demonstrates a solid foundation for Alzheimer’s stage classification.

### Model Explainability

- **Grad-CAM**: Used Gradient-weighted Class Activation Mapping (Grad-CAM) to generate heatmaps that visually highlight the regions of MRI images influencing the model’s predictions.
- **Transparency**: These visualizations ensure that the model's focus aligns with clinically relevant areas of the brain, providing transparency and building trust in the AI system.

## Ethical Considerations

- **Data Privacy**: Anonymized MRI data to safeguard individual identities and ensure confidentiality.
- **Fairness**: Represented all regions equitably to avoid bias and provide a balanced analysis.
- **Transparency**: Emphasized the importance of making the model’s decision-making process visible, avoiding the “black box” problem, and ensuring ethical AI deployment.




