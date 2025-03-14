Pneumonia Detection from Chest X-rays using Neural Networks
Overview
This project builds a neural network-based system for detecting pneumonia in chest X-ray images. It explores multiple deep learning architectures, including CNN, ResNet, VGGNet, and Inception, to classify X-ray images as either normal or pneumonia-infected. The study aims to enhance diagnostic accuracy using convolutional neural networks (CNNs) and transfer learning techniques.

Dataset
The dataset consists of 5,856 labeled chest X-ray images categorized as:

Pneumonia: 4,273 images
Normal: 1,583 images
To ensure balanced training, the pneumonia class was undersampled to 1,583 images. The dataset is sourced from Mendeley.

Methodology
Data Preprocessing & Augmentation

Image resizing
Rotation, flipping, and zooming to improve model generalization
Data standardization
Model Architectures Explored

CNN: Custom convolutional neural network
ResNet50: Pre-trained model with transfer learning
VGG19: Deep learning model leveraging transfer learning
InceptionV3: Advanced architecture using multi-scale feature extraction
Training Process

Loss function: Binary Cross-Entropy
Optimizers: Adam, RMSprop
Callbacks: Early stopping, model checkpointing
Performance Metrics: Accuracy, Precision, Recall
Results
Model	Validation Accuracy	Precision	Recall	Validation Loss
CNN	82.97%	86.64%	78.57%	0.454
ResNet50	94.01%	97.97%	94.26%	0.335
VGG19	90.48%	100%	80.00%	1.04
InceptionV3	89.27%	87.35%	92.24%	0.463
Best Model: ResNet50, achieving the highest accuracy and recall with minimal overfitting.

Conclusion
This project demonstrates the potential of deep learning models in pneumonia detection from chest X-rays. Among the evaluated models, ResNet50 emerged as the most reliable, providing a balance between accuracy, recall, and computational efficiency. This study highlights how AI can assist healthcare professionals in making faster and more accurate diagnoses.
