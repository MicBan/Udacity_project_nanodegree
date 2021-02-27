# Dog Breed recognition algorithm - Udacity Nanodegree
 Project to finalise the Udacity Data Scientist Nanodegree 
 
 ### Table of Contents
 
1. [Installation](#installation)
2. [Project Motivation](#motivation)
3. [Files Description](#files)
4. [Results](#results)
5. [Licensing, Authors, and Acknowledgements](#licensing)


## Installation <a name="installation"></a>

There should be no necessary libraries to run the code here beyond the Anaconda distribution of Python. The code should run with no issues using Python versions 3.\*. 

For completness, list libraries used in the project is listed below:
- sklearn
- keras
- numpy
- pandas
- glob
- cv2
- random
- matplotlib

Due to size restrictions there is missing a file DogVGG16Data.npz which should be normally found in the bottleneck_features folder. Also note that only a sample of available data has been uploaded on Github due to storage limitations.

It is highly recommended to run the Jupyter Notebook only when you have access to GPU due to performance issues should you run CNN on your CPU. When ru

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
- _data_, which consists of images used to train, validate and test model,
- _bottleneck_features_, including Resnet50 preprocessed inputs provided by Udacity. There should be also a respective file for VGG16 however due to storage limitations (it is 850mb of size) it could not be uploaded to Github
- _saved_models_, which includes parameters of the best models trained in this project
- _images_, including images feeding the Jupyter Notebook as well as a few used to test the result of the algorithm

## Results <a name="results"></a>
The result of this project are presented on a blog post (link). Additionally one can read the provided 'dog_app.html' to see all the steps I took and results achieved when I created a final version of this project.

Summing up, the accuracy of the model built by my from scratch reached **20.57%** after 30 epochs. The accuracy of model build on top of Resnet50 reached reasonable **80.74%**.

## Licensing, Authors, Acknowledgements<a name="licensing"></a>
Credit for provided data and structure of the project goes to Udacity.com and their partners. Concerning my code, feel free using is in line with the MIT licence.
