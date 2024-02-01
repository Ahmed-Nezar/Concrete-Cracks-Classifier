# Concrete-Cracks-Classifier

## Introduction
Crack detection has vital importance for structural health monitoring and inspection. We would like to train a network to detect Cracks, we will denote the images that contain cracks as positive and images with no cracks as negative.

Examples from the dataset:


![Negative_Sample](https://github.com/Ahmed-Nezar/Concrete-Cracks-Classifier/assets/125882735/83b5a623-92fa-4899-98c8-12e03d2f4211)    ![Positive_Sample](https://github.com/Ahmed-Nezar/Concrete-Cracks-Classifier/assets/125882735/a19956e3-be71-4559-a128-0de7251c5e30)
    

We used different models as below:
- ResNet50
- VGG16
- ResNet18

You will find in the repositry each model & the directories will be divided as follows:
- /models: contains the saved model after training
- /notebooks: contains the notebooks used for training

In each of the architectures mentioned above the fully connected layer was changed to classify the images into two classes (positive & negative) & the activation function we used was softmax.

## Dataset
The dataset used if from IBM capstone project of the professional cerificate [AI Engineering](https://www.coursera.org/professional-certificates/ai-engineer?) 

Dataset can be found from the following links:
- Data for ResNet50 & VGG16: [link](https://s3-api.us-geo.objectstorage.softlayer.net/cf-courses-data/CognitiveClass/DL0321EN/data/concrete_data_week3.zip)
- Data for ResNet18:
    - [Positive Tensors](https://s3-api.us-geo.objectstorage.softlayer.net/cf-courses-data/CognitiveClass/DL0321EN/data/images/Positive_tensors.zip)
    - [Negative Tensors](https://s3-api.us-geo.objectstorage.softlayer.net/cf-courses-data/CognitiveClass/DL0321EN/data/images/Negative_tensors.zip)

## Training
The below table will show the training for each model with the number of epochs & the accuracy achieved.

| Model |Optimizer| Epochs | Accuracy | loss|
| --- | --- | --- | --- | --- |
| ResNet50 | Adam | 2 | 0.9985 | 0.0061 |
| VGG16 | Adam | 2 | 0.9958 |  0.0188 |
| ResNet18 | Adam | 1 |  0.9943 | 23.88 |

## Evaluation
The evaluation was done on ResNet50 & VGG16 models, the evaluation was done on 1000 images for each model 

The ResNet50 model achieved an accuracy of 0.99906 & the VGG16 model achieved an accuracy of 0.99624 so overall the ResNet50 model performed better than the VGG16 model.

## Special Thanks
Special thanks to [IBM](https://www.ibm.com/) for providing the dataset & the course for the capstone project.
