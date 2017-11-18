# Semantic Segmentation
### Introduction
In this project, you'll label the pixels of a road in images using a Fully Convolutional Network (FCN).

### Approach
The Code can be found in the Jupyter notebook. [Semantic-Segmentation](Semantic-Segmentation.ipynb)

A VGG-16 network was converted to a fully convulation network.  Skip connection were used for a better performache. Based on this  implementation [ FCN-8 architecture](https://people.eecs.berkeley.edu/~jonlong/long_shelhamer_fcn.pdf)

Adam was used as a optimizer with cross-entropy loss function.

The hyperparameters used for training are:

keep_prob: 0.5
learning_rate: 0.0009
epochs: 30
batch_size: 5

Average loss was after 30 Epochs at 0.025. Performance is very good, but not perfect,

![](runs/traning_loss.png)

### Images 


![](runs/1510787455.012058/uu_000069.png)
![](runs/1510787455.012058/uu_000071.png)

![](runs/1510787455.012058/uu_000079.png)

![](runs/1510787455.012058/uu_000098.png)


![](runs/1510787455.012058/uu_000090.png)

![](runs/1510787455.012058/uu_000080.png)

### Setup
##### Frameworks and Packages
Make sure you have the following is installed:
 - [Python 3](https://www.python.org/)
 - [TensorFlow](https://www.tensorflow.org/)
 - [NumPy](http://www.numpy.org/)
 - [SciPy](https://www.scipy.org/)
##### Dataset
Download the [Kitti Road dataset](http://www.cvlibs.net/datasets/kitti/eval_road.php) from [here](http://www.cvlibs.net/download.php?file=data_road.zip).  Extract the dataset in the `data` folder.  This will create the folder `data_road` with all the training a test images.

### Start
##### Implement
Implement the code in the `main.py` module indicated by the "TODO" comments.
The comments indicated with "OPTIONAL" tag are not required to complete.
##### Run
Run the following command to run the project:
```
python main.py
```
**Note** If running this in Jupyter Notebook system messages, such as those regarding test status, may appear in the terminal rather than the notebook.

### Submission
1. Ensure you've passed all the unit tests.
2. Ensure you pass all points on [the rubric](https://review.udacity.com/#!/rubrics/989/view).
3. Submit the following in a zip file.
 - `helper.py`
 - `main.py`
 - `project_tests.py`
 - Newest inference images from `runs` folder  (**all images from the most recent run**)
 
 ## How to write a README
A well written README file can enhance your project and portfolio.  Develop your abilities to create professional README files by completing [this free course](https://www.udacity.com/course/writing-readmes--ud777).
