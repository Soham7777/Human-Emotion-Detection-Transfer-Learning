# Human Expression Detection with FER Dataset

This project focuses on detecting human emotions in grayscale images using transfer learning with a VGG19 model. The dataset used is the FER (Facial Expression Recognition) dataset, which consists of 48x48 pixel grayscale images of faces categorized into seven emotions (0=Angry, 1=Disgust, 2=Fear, 3=Happy, 4=Sad, 5=Surprise, 6=Neutral).

## Dataset

- The dataset comprises 28,709 training examples and 3,589 test examples.
- All images are centered and standardized to 48x48 pixels.
- Emotions are categorized into seven classes.


## Transfer Learning

### Goal

The goal of this project was to leverage transfer learning by using a VGG19 model pre-trained on the Imagenet dataset to improve performance compared to standard models.

### Model Configuration

- Optimizer: SGD
- Learning Rate: 0.001
- Loss Function: Categorical Crossentropy
- Batch Size: 32
- Epochs: 50
- Data Augmentation

### Model Insights

1. A VGG19 model was used with the first two CNN blocks frozen to retain Imagenet weights, while the other layers were trained using the FER dataset.
2. Data augmentation was applied before feeding data to the model to handle increased model complexity and improve predictability for unseen and real-time data.
3. The model was trained for 50 epochs with early stopping callbacks to prevent overfitting.
4. The overall accuracy achieved was 0.64 as measured by F1-score.
5. The project report attached as a PDF contains more detailed insights, including model parameters, training graphs, F1 scores, and sample predictions.

For a more comprehensive report, please refer to the [link-to-report.pdf](https://github.com/Soham7777/Human-Emotion-Detection-Transfer-Learning/blob/main/Report.pdf).

## Dataset Source

- [Facial Expression Recognition (FER) Challenge | Kaggle](https://www.kaggle.com/c/challenges-in-representation-learning-facial-expression-recognition-challenge/data)

## Technical Details

- Image Size: 48x48x3 (Modified for Transfer Learning models)
- Optimizer: SGD
- Learning Rate: 0.001
- Loss Function: Categorical Crossentropy
- Batch Size: 32
- Epochs: 50
- Data Augmentation

