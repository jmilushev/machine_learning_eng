# Capstone project - Distracted Drivers Detection

A dataset of images is used to create a deep neural network model to classify each image into 1 of 10 categories. A pretrained model (MobileNetV2) is used which was trained on the provided dataset. The hyper parameters are optimized using grid search and image augmentation is utilized in an attempt to reduce overfitting. Overall the achieved result is better than 75% of the participants in a Kaggle competition taken place about 2 years earlier.

## Getting Started

1. clone the files from this repo into a location on your computer;
2. download the datasets from the Kaggle competion "State Farm Distracted Driver Detection". Unzip the imgs.zip file and move under project_files/data/imgs/test and project_files/data/imgs/train
3. create a conda virtual encironment with the following dependencies:

* python 3.6
* numpy 1.14.3
* pandas 0.23.0
* seaborn 0.9.0
* keras 2.2.4
* tensorflow 1.11.0
* scikit-learn 0.19.1
* tqdm 4.28.1

You may utilize conda virtual environments and create an environment called *distracted_drivers_env* on MacOs using the included environment file, by executing:

```
cd project_files
conda create --name distracted_drivers_env --file requirements/distracted_drivers_mac.txt
```

### Junyper Notebooks

* **analyze data** - analyzes the training data sets
* **pre-process data** - prepares the dayasets in the desired format and saves to project_files/data/tensors
* **optimize hyper parameters for MobileNet V2 model** - uses scikit-leanrn Grid Search to optimize hyper paramaters
* **train MobileNet V2 model** - trains the MobileNetV2 model using the optimized hyper parameters


