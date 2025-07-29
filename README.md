# Brain-tumor-classification-using-CNN-Transfer-Learning
This repository presents a brain tumor classification system using advanced Convolutional Neural Networks (CNN) and Transfer Learning (ResNet50 and Xception). The model classifies MRI brain images into four classes: Glioma, Meningioma, Pituitary Tumor, and No Tumor, aiming to support medical diagnostics through deep learning and image analysis.

## Objectives
- Develop a CNN-based model for multi-class brain tumor classification.
- Compare baseline model with advanced CNN and pre-trained models.
- Evaluate model performance using precision, recall, F1-score, and accuracy.
- Apply transfer learning (ResNet50 & Xception) to enhance classification accuracy.
- Analyze misclassification patterns and improve feature learning.

## Model Architectures
1. Advanced CNN
   - 4 Convolutional Blocks (16–128 filters)
   - ReLU, MaxPooling, Dropout (0.25)
   - Dense layer (128 neurons) + Dropout
   - Output: Softmax (4 classes)
   - Optimizer: Adam (lr = 0.0001)
2. Transfer Learning Method
   - Xception and ResNet 50
   - Pretrained on ImageNet
   - Custom top layers with Flatten → Dense(128) → Dropout → Softmax
   - Frozen base layers
   - Optimizer: Adamax (lr = 0.001)
  
## Results
1. Advanced CNN
   - Accuracy: 94%
   <img width="469" height="409" alt="image" src="https://github.com/user-attachments/assets/1ac192f1-96e5-4596-8dab-4469c3ce20f7" />

2. Xception (Transfer Learning)
   - Accuracy: 98%
   <img width="469" height="409" alt="image" src="https://github.com/user-attachments/assets/d4061ce9-1a7b-4a49-a360-83b812359ac2" />

## Key Insights
- Data expansion and augmentation significantly improved generalization.
- Transfer learning models like Xception outperform traditional CNNs.
- Glioma tumors remain challenging due to overlapping features with no-tumor class.
- Regularization techniques (dropout) and optimized hyperparameters played a key role.

