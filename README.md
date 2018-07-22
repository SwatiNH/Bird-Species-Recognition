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

#### Advantages
* It gains flexibility in the choice of the form of the threshold.  
* Contains a nonlinear transformation.  
* It provides a good generalization capability.  The problem of overfitting is eliminated.  
* Reduction in computational complexity.  Simple to manage decision rule complexity and Error frequency.

#### Disadvantages 
Result transparency is low. Training is time consuming.  Structure of algorithm is difficult to understand Determination of optimal parameters is not easy when there is nonlinearly separable training data.


### Convolutional Neural Network

#### Description 
* CNN compare images piece by piece. By finding approximate matching features in same positions in the two images, it’s performs better those schemes that simply matching the two images as a whole. 
* Filtering is used to match features with the image patch. The convolutional aspect involves repetitive matching in every possible way. Each image becomes a stack of filtered images. ReLU is a used to normalise the values. 
* Pooling involves shrinking the stack size by taking strides of fixed length and picking the highest values in each window. The above process is repeated many times to form deep stacking of layers. 
* Backpropagation could be used to improve accuracy over iterations, and for this we need a collection of images for which we know the answer.

