# Strabismus-Detection-System

This project implements an automated classification system for strabismus detection using deep convolutional neural networks. It aims to assist clinical diagnosis by classifying eye images into five categories: Exotropia, Esotropia, Hypertropia, Hypotropia, and Normal.

The dataset consists of clinically sourced eye images, preprocessed via auto-orientation, resizing (224x224), and denoising. Augmentation techniques such as flipping, brightness tuning, contrast enhancement, and grayscale conversion were applied to the training data. Data was split into training, validation, and testing sets in a 70:15:15 ratio.

Eight CNN models were trained and evaluated: AlexNet, VGGNet19, ResNet50, Inception-ResNetV2, EfficientNetB7, DenseNet121, MobileNetV2, and a custom ConvNet. All models were fine-tuned using Adam optimizer and categorical cross-entropy loss, with evaluation metrics including accuracy, precision, recall, and F1-score.

EfficientNetB7 achieved the best results with 84% accuracy. MobileNetV2 and ResNet50 followed with 77% and 74% accuracy respectively. The system is optimized for deployment in low-resource settings and supports potential integration into mobile or embedded platforms.

Key contributions include architecture implementation, dataset curation, augmentation strategy design, and hyperparameter tuning.
