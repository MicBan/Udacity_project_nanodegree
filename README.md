# Dog Breed recognition algorithm - Udacity Nanodegree
 Project to finalise the Udacity Data Scientist Nanodegree 
 
 ### Table of Contents
 
1. [Installation](#installation)
2. [Project Motivation](#motivation)
3. [Files Description](#files)
4. [Results](#results)
5. [Licensing, Authors, and Acknowledgements](#licensing)


## Installation <a name="installation"></a>


It is highly recommended to run the Jupyter Notebook only when you have access to GPU due to performance issues should you run CNN on your CPU. On your machine you should have installed Python 3.\* with Anaconda packages, ensuring that the following libraries are also available (where keras is the single most important one):
- sklearn
- keras
- numpy
- pandas
- glob
- cv2
- random
- matplotlib

Due to size restrictions there is missing a file DogVGG16Data.npz which should be normally found in the bottleneck_features folder. For this reason a part of the code won't work however that does not impact the final algorithm.
Note that there are missing data due to Udacity project submission requirements.

## Project Motivation<a name="motivation"></a>

My main motivation behind this project is concerning development of skills in regards to neural networks and deep learning. Specifically, here I try to learn the following:

1. How to create a CNN from scratch?
2. How to apply transfer learning?
3. How change of parameters impacts accuracy of predictions?

## Files description<a name="files"></a>
The core file is Jupyter Notebook file named 'dog_app.ipynb' which includes a core result of this project, i.e. code describing CNN used to analyse images.
Apart from that there are following files in the main folder which need mentioning:
- 'dog_app.html' - HTML version of the Jupyter Notebook, showing a stable version of the project
- 'extract_bottleneck_features.py' - file provided by Udacity, used to read pretrained models provided by Keras using provided preprocessed inputs

Other important folders include:
- _data_, which should consists of images used to train, validate and test model, but is empty to allow the project to be submitted,
- _bottleneck_features_, including Resnet50 preprocessed inputs provided by Udacity. There should be also a respective file for VGG16 however due to storage limitations (it is 850mb of size) it could not be uploaded to Github
- _saved_models_, which includes parameters of the best models trained in this project
- _images_, including images feeding the Jupyter Notebook as well as a few used to test the result of the algorithm

## Results <a name="results"></a>
The result of this project are presented on a [blog post](https://medium.com/@banach.michal/ouch-whats-that-or-how-to-apply-cnn-to-identify-dog-breed-af94c52d7d12). Additionally one can read the provided 'dog_app.html' to see all the steps I took and results achieved when I created a final version of this project.

Summing up, the accuracy of the model built by my from scratch reached **5.14%** after just 5 epochs. The accuracy of model build on top of Resnet50 reached reasonable **79.30%** after 20 epochs.

## Licensing, Authors, Acknowledgements<a name="licensing"></a>
Credit for provided data and structure of the project goes to Udacity.com and their partners. Concerning my code, feel free using is in line with the MIT licence.
