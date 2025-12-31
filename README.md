# AQREIGHT-CV-ENGINEER-TECHNICAL-ASSESSMENT
## Applicant Name : Ahmad Zhafri Hariz Bin Roslan
This repo is for AQREIGHT CV Engineer Assessment 


# Overview
This assessment was done on the Flower102 dataset for image classification task.
There are 3 notebooks present within this repo:
- EDA.ipynb
- Traning.ipynb
- Evaluation_and_Explainability.ipynb

# Approach
EDA : My approach for this assessment are based on the EDA analysis where the dataset shows a high contrast and class imbalances on the test dataset which reflect my data augmentation.

Data Pipeline: A heavy data augmentation was utilized to help the model to generalize better in the imbalance dataset

Transfer Learning Model : A full fine-tune model was employ. I compare 3 models; ResNet50, ViT, and ConvNext-tiny for model selection. This approach would compare the 3 models in terms of their accuracy on the testing dataset. These 3 models are considered as the most commonly used models for image classification where ResNet is the Golden standard, ViT uses transformer and attention mechanism to understand gobal context and ConvNext is the modernize CNN architecture.

Training Infrastructure : Early stopping and model checkpointing was implemented. The training metrics (loss, accuracy, val_loss, val_accuracy, and learning rate) was logged.

Model Selection : From the models that are trained, the ConvNext-tiny shows the highest performance in terms of accuracy. The model is used for further evaluation.

Evaluation : The ConvNext achieved 94.44% Precision, Recall 93.76%, Accuracy 93.76%, F1-Score 93.79%
