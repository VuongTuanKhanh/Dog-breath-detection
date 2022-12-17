# Dog Breed Classification

## Content:
- [Project Description](#project-description)
- [Files](#files)
- [Installation Instruction](#installation-instruction)
- [Usage Instruction](#usage-instruction)



The Notebook contains the [REPORT](.report\detection_report.html) required for this project.

## Project Description
This is the Capstone project for the Udacity Data Science Nanodegree course.
For the packages used in the project, please take a look at [requirements file](requirements.txt)

### Project Overview
This project will accept any user-supplied image as input.  If a dog is found in the photograph, an estimate of the breed will be given. When a human image is found, an estimation of the person who it most closely resembles is given.

### Problem Statement
Every important breed has its own sub-breeds and distinguishing characteristics, such as fur color, texture, head form, ear shape, and facial expression. If all we can see are pictures of dogs, it's even more difficult.
The main goal is to utilize the power of CNN model that can predict the breed with the highest degree of accuracy from an input RGB image of a dog. Simply evaluating a few models (VGG16, ResNet50, VGG19, and my own model) will allow me to get a foundational understanding of computer vision in data science.

### Metrics
Since this is a classification problem, evaluation is based on accuracy. Basically, the model is evaluated on the test set and in percentage.


## Files
```
Dog_breed_detection
│   README.md
│   requirements.txt // required packages
|	LICENSE.txt
│
└───app
│   │   dog_app.py
|	|	run.py
│   │
│   └───upload_folder // contains images uploaded from users
│   │
│   └───templates // contains HTML template files for the webapp.
│       │   index.html
│   
└───bottleneck_features
│   │   DogVGG16Data.npz
│   │   DogResnet50Data.npz
│
└───haarcascades
│   │   haarcascade_frontalface_alt.xml // model to detect human faces
│
└───notebook
|   |   images
│   │   dog_app.ipynb
|	|	download_workspace.ipynb
|	|	extract_bottleneck_features.py
|
└───report
|	|	detection_report.html // HTML report file 
|
└───sample_images // list of sample images use for detection
|	
└───saved_models //contains saved data for dog breed identification model developed in the notebook
│   │   weights.best.from_scratch.hdf5
|	|	weights.best.Resnet50.hdf5
|	|	weights.best.VGG16.hdf5
│
```

## Installation Instruction
Once you have pull the repo, or download and unzip this repo, please follow the step below to complete the setup.

- Setup an environment (>= Python 3.6) and install packages from [requirements file](requirements.txt).

## Usage Instruction
- After installing the packages, simply run `python run.py` and point you browser to http://127.0.0.1:8080/. The app itself is self-explanatory.
