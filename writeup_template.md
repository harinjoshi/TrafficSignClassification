# **Traffic Sign Recognition using neural network** 

This project aims at classifying traffic signs using image processing techniques and using neural networks.

---

Following are the dependencies(Python Packages required):
[Matplotlib](http://matplotlib.org/)
[numpy](http://www.numpy.org/)
[jupyter](http://jupyter.org/)
[scikit-learn](http://scikit-learn.org/)
[Tensorflow](http://tensorflow.org)

### Note: Install miniconda if running on local machine it comes with very basic structure to load python without installation of any package.

Install above packages as per requirement.


**Build a Traffic Sign Recognition Project**

The goals / steps of this project are the following:
* Load the data set (see below for links to the project data set)
 [Download the dataset](https://d17h27t6h515a5.cloudfront.net/topher/2016/November/581faac4_traffic-signs-data/traffic-signs-data.zip). This is a pickled dataset in which we've already resized the images to 32x32.
 
* Explore, summarize and visualize the data set

* Design, train and test a model architecture

* Use the model to make predictions on new images

* Analyze the softmax probabilities of the new images

* Summarize the results with a written report

Above steps are to be followed from jupyter notebook for this project

### Data Set Summary & Exploration

#### 1. 
I used the pandas shape methodd to calculate summary statistics of the traffic
signs data set:

* The size of training set is  34799
* The size of the validation set is  4410
* The size of test set is 12630
* The shape of a traffic sign image is (32, 32, 3)
* The number of unique classes/labels in the data set is 43


### Design and Test a Model Architecture

#### checkout [traffic-sign-notebook](https://github.com/harinjoshi/TrafficSignClassification/blob/master/Traffic_Sign_Classifier.ipynb) to undersrtand how data has been preprocessed,training data with validation and test sets.

#### 2. Describe what your final model architecture looks like including model type, layers, layer sizes, connectivity, etc.) Consider including a diagram and/or table describing the final model.

My final model consisted of the following layers:

| Layer         		|     Description	        					| 
|:---------------------:|:---------------------------------------------:| 
| Input         		| 32x32x3 RGB image   							| 
| Convolution 3x3     	| 1x1 stride, same padding, outputs 32x32x64 	|
| RELU					|												|
| Max pooling	      	| 2x2 stride,  outputs 16x16x64 				|
| Convolution 3x3	    | etc.      									|
| Fully connected		| etc.        									|
| Softmax				| etc.        									|
|						|												|
|						|												|
 


My final model results were:
* training set accuracy of= *0.999*
* validation set accuracy of= *0.944*
* test set accuracy of= *0.934*

### Testing a Model on New Images
The model was able to correctly guess 7 to 10 of the 19 traffic signs, which gives an accuracy in range 36%-52%. This compares favorably to the accuracy on the test set of ...

#### 3. Describe how certain the model is when predicting on each of the five new images by looking at the softmax probabilities for each prediction. Provide the top 5 softmax probabilities for each image along with the sign type of each probability.
On the left is given images, and it calculates top 5 possibilities of given images as classified by model.
probability of 1.0 is highest possible match among all other probable candidates.
