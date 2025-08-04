# Smoker Detection
This project builds a deep learning pipeline to classify images into two categories: Smoking and Not Smoking. It uses transfer learning with DenseNet121 and a custom image augmentation pipeline for better generalization.
- The codes and examples can be found in [Smoker_detection.ipynb](https://github.com/bachPN73/Smoker-Detection/blob/main/Smoker_detection.ipynb).
## The Dataset
Dataset link & Credit: [https://www.kaggle.com/datasets](https://www.kaggle.com/datasets/phamngocbach73/smoker-1k2)
- Training/
### ├── smoking_001.jpg
### ├── notsmoking_002.jpg
### └── ...

- The dataset contains 1120 images divided equally into two classes, where 560 images are of Smoking and remaining 560 images belong to NotSmoking class

- Not smoking
![Result](Sample%20Data/notsmoking_0320.jpg)

- Smoking
![Result](Sample%20Data/smoking_0464.jpg)

## Training
### Uses DenseNet121 (pretrained) + custom top layers.
### Trained in 2 phases:
- Freeze base
- Fine-tune last 30 layers
## Evaluation
### After training and fine-tuning, the model reaches a final accuracy on the test set:
Accuracy model: 0.92
## Result
![Result](Sample%20Data/Screenshot%202025-08-04%20102632.png)

