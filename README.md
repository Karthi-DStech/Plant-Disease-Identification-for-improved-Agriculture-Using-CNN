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
