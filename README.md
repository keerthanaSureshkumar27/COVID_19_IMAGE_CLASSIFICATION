# COVID-19 Image Classification Using CNN

## Project Overview
This project uses a Convolutional Neural Network (CNN) to classify chest X-ray images into two categories: **COVID-19** and **Normal**. The objective is to explore how deep learning can support medical image classification and assist healthcare professionals in preliminary screening.

## Objectives
- Classify chest X-ray images as COVID-19 or Normal.
- Build and compare two CNN models.
- Evaluate model performance using accuracy and COVID-19 recall.
- Understand overfitting and improve model generalization.

## Dataset
- **Total Images:** 251
- **Image Size:** 128 × 128 pixels
- **Image Format:** RGB
- **Classes:** COVID-19 (1) and Normal (0)
- **Data Split:** 70% Training, 15% Validation, 15% Testing

The images were normalized by scaling pixel values from 0–255 to 0–1.

## Technologies Used
- Python
- NumPy and Pandas
- Matplotlib and Seaborn
- OpenCV
- TensorFlow and Keras
- Scikit-learn

## Project Workflow
1. Load chest X-ray images and their labels.
2. Perform exploratory data analysis and visualize class distribution.
3. Resize and normalize images for model training.
4. Split the dataset into training, validation, and testing sets.
5. Build and train two CNN models.
6. Evaluate model performance using accuracy and recall.
7. Compare the models and select the preferred model based on performance and generalization.

## Model Architecture

### Model 1
- Three convolutional layers with 32, 64, and 128 filters.
- Max pooling layers.
- Flatten layer.
- Dense layer with 128 neurons and ReLU activation.
- Sigmoid output layer for binary classification.

### Model 2
- Two convolutional layers with 32 and 64 filters.
- Max pooling layers.
- Flatten layer.
- Dense layers with 128 and 64 neurons using ReLU activation.
- Sigmoid output layer.
- Adam optimizer with a learning rate of 0.0001.

## Evaluation
The models were evaluated using accuracy and COVID-19 recall. Model 1 showed signs of overfitting, so Model 2 was explored as an alternative to improve generalization. The preferred model was selected with particular attention to COVID-19 recall, since missing positive cases is an important concern in medical screening.

*Note: Add the final test-set accuracy, precision, recall, and F1-score after confirming the actual evaluation results.*

## Key Learnings
- Understanding CNN architecture and image classification.
- Image preprocessing and normalization.
- Training and evaluating deep learning models.
- Identifying overfitting and comparing model architectures.
- Understanding the importance of recall in medical classification.

## Future Improvements
- Increase the size and diversity of the dataset.
- Apply data augmentation to improve generalization.
- Use additional evaluation metrics and confusion matrices.
- Test the model on an independent dataset.
- Explore transfer learning using pretrained CNN architectures.

## Disclaimer
This project is for educational purposes only. It is not intended to diagnose COVID-19 or replace professional medical evaluation.

## Author
**Keerthana Sureshkumar**

B.Sc. Data Science
