# Bird-Species-Recognition
Machine Learning Project
## Problem Statement

Building an optimal Bird Species Classifier.


## Dataset details


### Dataset
Caltech-UCSD Birds-200-2011 (CUB-200-2011) is an extended version of the CUB-200 dataset, with roughly double the number of images per class and new part location annotations. For detailed information about the dataset, please see the technical report linked below.

#### Number of categories
* 200 catergories
#### To name a few
* Black_footed_Albatross
* Laysan_Albatross
* Sooty_Albatross
* Parakeet_Auklet
* Rhinoceros_Auklet
* Brewer_Blackbird

#### Number of images
* 11,788

#### List of attributes
Total 312 binary attributes
To name a few
* has_bill_shape::curved_(up_or_down)
* 10 has_wing_color::blue
* has_upperparts_color::blue
* has_breast_pattern::spotted
* has_back_color::brown
* has_tail_shape::forked_tail


### Support Vector Machines

#### Description  
A support vector machine builds a hyperplane or set of hyperplanes in a high- or infinite dimensional space, used for classification. Good separation is achieved by the hyper plane that has the largest distance to the nearest training data point of any class (functional margin), generally larger the margin lower the generalization error of the classifier.

#### Characteristics 
SVM uses Nonparametric with binary classifier approach and can handle more input data very efficiently. Performance and accuracy depends upon the hyperplane selection and kernel parameter.


### Convolutional Neural Network

#### Description 
* CNN compare images piece by piece. By finding approximate matching features in same positions in the two images, it’s performs better those schemes that simply matching the two images as a whole. 
* Filtering is used to match features with the image patch. The convolutional aspect involves repetitive matching in every possible way. Each image becomes a stack of filtered images. ReLU is a used to normalise the values. 
* Pooling involves shrinking the stack size by taking strides of fixed length and picking the highest values in each window. The above process is repeated many times to form deep stacking of layers. 
* Backpropagation could be used to improve accuracy over iterations, and for this we need a collection of images for which we know the answer.

#### Characteristics 
The hyper parameters that the user has to feed to the network are
##### Convolution 
* Number of features
* Size of features
##### Pooling
* Window size
* Window stride
##### Fully Connected
* Number of neurons.

An inception model is a CNN which uses convolution kernels of multiple sizes as well as pooling within one layer. As it turns out this yields very good results because hierarchical information with varying sizes can be identified at the same layer. Plus the fact that you don't have to worry about setting kernel sizes so rigidly because many different size are used. It is always good to have a general rule like this instead of a hyper parameter.

### Design of model
* Transfer Learning
It is a technique in which a model trained on one task is purposed on another task. Transfer learning is an optimization that allows rapid progress or improved performance when modeling the second task.

#### How to Use Transfer Learning?
You can use transfer learning on your own predictive modeling problems. Two common approaches are as follows:
* Develop Model Approach
* Pre-trained Model Approach

#### Pre-trained Model Approach
* Select Source Model. 
A pre-trained source model is chosen from available models. Many research institutions release models on large and challenging datasets that may be included in the pool of candidate models from which to choose from.
* Reuse Model. 
The model pre-trained model can then be used as the starting point for a model on the second task of interest. This may involve using all or parts of the model, depending on the modeling technique used. 
* Tune Model. 
Optionally, the model may need to be adapted or refined on the input-output pair data available for the task of interest.
One of the techniques in our project involved Transfer Learning with Image Data. So for we used pre-trained ImageNet model, for running *Inception Classification technique 

