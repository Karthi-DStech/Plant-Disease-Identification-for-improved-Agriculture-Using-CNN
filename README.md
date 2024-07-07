# Plant-Disease-Identification-for-improved-Agriculture-Using-CNN

This project focuses on the application of deep learning to identify and classify plant diseases, which is a major challenge in the agricultural sector with serious implications for crop yield and food supply. Our research evaluates various Convolutional Neural Network (CNN) architectures, combined with data augmentation techniques and optimizers, to develop a robust solution for the detection of plant diseases through image classification.

### ****Models Evaluated****

- **AlexNet**: One of the pioneer deep learning architectures known for its success in large-scale image recognition challenges.
- **DenseNet121**: Utilizes dense connections to ensure maximum information flow between layers in the network.
- **EfficientNetB0**: Focuses on optimizing the scaling of depth, width, and resolution of the network for better performance.
- **MobileNetV2**: Designed for mobile and embedded vision applications, known for its lightweight structure and efficiency.
- **ResNet50**: Employs residual connections to enable training of very deep networks by mitigating the vanishing gradient problem.
- **VGG16**: Characterized by its simplicity, using only 3x3 convolutional layers stacked on top of each other in increasing depth.
- **Custom CNN Architecture**: A bespoke model developed to serve as a baseline for performance comparison.

### **Ensembling Techniques**

- **Average Ensemble**: An ensemble method that averages the predictions of multiple models to improve accuracy.
- **Voting Ensemble**: This technique aggregates the predictions of each model based on majority voting, providing robust performance against overfitting.

### **Key Techniques and Strategies**

- **Data Augmentation**: Implemented to artificially expand the training dataset and improve model generalizability.
- **Optimizers**: Explored different optimizers, with AdaBelief optimizer emerging as a top performer in conjunction with our chosen models.

### ****Results and Findings****

- The project's highlight is the development of an ensemble method combining two predictions of  DenseNet121 and ResNet50 models, which achieved a record accuracy of 99.94%.
- Comparative analysis of the models showed that ensemble methods substantially improve accuracy and robustness.

## **Repository Structure**

Our repository is organized as follows:

### **Models and Scripts**

**`Alex-Net`**
- `Alexnet_SGD.py`: Script for training the AlexNet model using SGD optimizer.

**`Dense-Net`**
- `Densenet121_SGD.py`: Script for training DenseNet121 with SGD optimizer.
- `Densenet121_adabelief.py`: DenseNet121 trained with AdaBelief optimizer.

**`Efficient-Net`**
- `EfficientnetB0_SGD.py`: Script for EfficientNetB0 with SGD optimizer.
- `EfficientnetB0_adabelief.py`: EfficientNetB0 optimized with AdaBelief.

**`Mobile-Net`**
- `MobilenetV2_SGD.py`: MobileNetV2 training script using SGD optimizer.
- `MobilenetV2_adabelief.py`: MobileNetV2 using the AdaBelief optimizer.

**`Res-Net`**
- `Resnet50_SGD.py`: Training script for ResNet50 with SGD.
- `Resnet50_adam.py`: Adam optimizer script for ResNet50.

**`VGG`**
- `VGG16_SGD.py`: Script to train VGG16 with SGD optimizer.
- `VGG16_adam.py`: VGG16 training with Adam optimizer.

**`Custon-CNN`**
- `custom_CNN_adam.py`: Custom CNN architecture trained with Adam optimizer.

### **Ensemble Models**

**`Voting-Emsemble`**
- `Voting_Ensemble_2base.py`: Script for a 2-model voting ensemble.
- `Voting_Ensemble_4base.py`: 4-model voting ensemble training script.

**`Emsemble-Dense`**
- `Ensemble_Densenet121_2base.py`: A 2-model ensemble with DenseNet121 architectures.

**`Emsemble-Efficient`**
- `Ensemble_EfficientnetB0_2base.py`: EfficientNetB0 duo in an ensemble setup.
- `Ensemble_EfficientnetB0_4base.py`: Ensemble script for four EfficientNetB0 models.

### **Output Logs**

- **`.out`** files corresponding to each **`.py`** script provides the training and validation logs for the models. 
